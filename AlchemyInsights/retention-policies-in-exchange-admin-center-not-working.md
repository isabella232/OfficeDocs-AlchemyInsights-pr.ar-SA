---
title: سياسات الاحتفاظ في مركز إدارة Exchange لا تعمل
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: e2fb22f872be0eefc3b4b78b18cd09baffa66cda
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742420"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d1c3b-102">سياسات الاحتفاظ في مركز إدارة Exchange</span><span class="sxs-lookup"><span data-stu-id="d1c3b-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="d1c3b-103">**المشكلة:** لا يتم تطبيق نُهج الاحتفاظ التي تم إنشاؤها أو تحديثها حديثًا في مركز Exchange Admin على صناديق البريد أو العناصر التي لا يتم نقلها إلى صندوق بريد الأرشيف أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d1c3b-104">**الأسباب الجذرية:**</span><span class="sxs-lookup"><span data-stu-id="d1c3b-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="d1c3b-105">قد يكون هذا بسبب لم يعالج **"مساعد المجلد المدار"** علبة بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d1c3b-106">يحاول "مساعد المجلد المدار" معالجة كل علبة بريد في المؤسسة المستندة إلى مجموعة النظراء مرة كل سبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="d1c3b-107">إذا قمت بتغيير علامة الاحتفاظ أو تطبيق نهج استبقاء مختلف على علبة بريد، يمكنك الانتظار حتى يعالج "مساعدة المجلد المدارة" علبة البريد، أو يمكنك تشغيل cmdlet بدء التشغيل المدارة FolderAssistant لبدء تشغيل "مساعد المجلد المدارة" لمعالجة علبة بريد معينة.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="d1c3b-108">تشغيل هذا cmdlet مفيد لاختبار أو استكشاف الأخطاء وإصلاحها نهج الاحتفاظ أو إعدادات علامة الاحتفاظ.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="d1c3b-109">لمزيد من المعلومات، قم [بزيارة تشغيل مساعد المجلد المدار](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="d1c3b-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d1c3b-110">**الحل:** تشغيل الأمر التالي لبدء تشغيل "مساعد المجلد المدارة" لعلبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="d1c3b-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d1c3b-111">قد يحدث هذا أيضاً إذا تم **تمكين** **RetentionHold** على علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d1c3b-112">إذا تم وضع علبة البريد على HoldHold، لن تتم معالجة نهج الاحتفاظ على علبة البريد خلال ذلك الوقت.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="d1c3b-113">لمزيد من المعلوماتية على إعداد RetentionHold انظر: [احتجاز الاحتفاظ بعلبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="d1c3b-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d1c3b-114">**حل:**</span><span class="sxs-lookup"><span data-stu-id="d1c3b-114">**Solution:**</span></span>
    
  - <span data-ttu-id="d1c3b-115">تحقق من حالة إعداد RetentionHold على علبة بريد محددة في [EXO powershell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)</span><span class="sxs-lookup"><span data-stu-id="d1c3b-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d1c3b-116">تشغيل الأمر التالي **لتعطيل** RetentionHoldعلى علبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="d1c3b-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d1c3b-117">الآن، إعادة تشغيل "مساعد المجلد المدارة":</span><span class="sxs-lookup"><span data-stu-id="d1c3b-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d1c3b-118">**ملاحظة:** إذا كان علبة البريد أصغر من 10 ميغابايت، لن يقوم "مساعد المجلد المدار" بمعالجة علبة البريد تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="d1c3b-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d1c3b-119">لمزيد من المعلومات حول نُهج الاحتفاظ في مركز إدارة Exchange، راجع:</span><span class="sxs-lookup"><span data-stu-id="d1c3b-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="d1c3b-120">علامات الاحتفاظ وسياسات الاحتفاظ</span><span class="sxs-lookup"><span data-stu-id="d1c3b-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="d1c3b-121">تطبيق نهج الاحتفاظ على علب البريد</span><span class="sxs-lookup"><span data-stu-id="d1c3b-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="d1c3b-122">إضافة علامات الاحتفاظ أو إزالتها</span><span class="sxs-lookup"><span data-stu-id="d1c3b-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="d1c3b-123">كيفية تحديد نوع الانتظار الموضوع على علبة بريد</span><span class="sxs-lookup"><span data-stu-id="d1c3b-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
