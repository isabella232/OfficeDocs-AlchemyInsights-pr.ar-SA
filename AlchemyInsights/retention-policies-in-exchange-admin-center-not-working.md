---
title: نهج الاستبقاء في مركز مسؤول Exchange لا يعمل
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 73e8db432afccb73b872ec7a3ce84c25f1ba7f25
ms.sourcegitcommit: ca06ef831226d629de3057a0df85e017b80f3356
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/08/2019
ms.locfileid: "29786757"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="e1374-102">نهج الاستبقاء في مركز مسؤول Exchange</span><span class="sxs-lookup"><span data-stu-id="e1374-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="e1374-103">**المشكلة:** المنشأة حديثا أو لا تطبق نهج الاستبقاء حدثت في مركز مسؤول Exchange إلى علب البريد أو عناصر نقل أرشيف علبة البريد أو حذفه لا.</span><span class="sxs-lookup"><span data-stu-id="e1374-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="e1374-104">**الأسباب الأساسية:**</span><span class="sxs-lookup"><span data-stu-id="e1374-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="e1374-p101">قد يرجع هذا **مساعد المجلد المدار** غير عالجت علبة بريد المستخدم. مساعد المجلد المدار يحاول معالجة كل علبة البريد في المؤسسة الخاصة بك إلى مجموعة النظراء مرة كل سبعة أيام. إذا غيرت علامة استبقاء أو تطبيق نهج استبقاء مختلفة لعلبة بريد، يمكنك الانتظار حتى "إدارة مجلد مساعدة" العمليات علبة البريد، أو يمكنك تشغيل الأمر cmdlet ماناجيدفولديراسيستانت ابدأ لبدء إدارة "مساعد المجلدات" لمعالجة معينة علبة البريد. تشغيل cmdlet هذا مفيداً لاستكشاف نهج استبقاء أو إعدادات علامة استبقاء أو الاختبار. لمزيد من المعلومات، قم بزيارة [تشغيل إدارة "مساعد المجلدات"](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="e1374-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="e1374-110">**الحل:** قم بتشغيل الأمر التالي لتشغيل إدارة "مساعد المجلدات" لعلبة بريد محددة:</span><span class="sxs-lookup"><span data-stu-id="e1374-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="e1374-p102">هذا قد أيضا يحدث إذا تم **تمكين** على صندوق البريد **ريتينتيونهولد** . إذا تم وضع علبة البريد في ريتينتيونهولد، لن تتم معالجة نهج الاستبقاء في علبة البريد خلال تلك الفترة. لمعلومات أكثر راجع الإعداد ريتينتيونهولد: [اضغط الاحتفاظ بعلبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="e1374-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="e1374-114">**الحل:**</span><span class="sxs-lookup"><span data-stu-id="e1374-114">**Solution:**</span></span>
    
  - <span data-ttu-id="e1374-115">التحقق من حالة الإعداد ريتينتيونهولد في علبة بريد معينة في [أكسو powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="e1374-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="e1374-116">تشغيل الأمر التالي **تعطيل** ريتينتيونهولد على علبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="e1374-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="e1374-117">والآن، إعادة تشغيل مساعد المجلد المدارة:</span><span class="sxs-lookup"><span data-stu-id="e1374-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="e1374-118">**ملاحظة:** إذا كانت علبة بريد أصغر من 10 ميغابايت، "مساعد المجلد المدار" سوف لا تلقائياً معالجة علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="e1374-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

