---
title: نُهج الاستبقاء في مركز إدارة Exchange لا تعمل
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
ms.openlocfilehash: 4d3ca121c8d22a0900f136f7f2a754dfb5b435f5
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522794"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="6f50c-102">نُهج الاستبقاء في مركز إدارة Exchange</span><span class="sxs-lookup"><span data-stu-id="6f50c-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="6f50c-103">إذا كنت تريد منا تشغيل الشيكات التلقائية للإعدادات المذكورة أدناه، حدد زر العودة <-- في أعلى هذه الصفحة، ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي لديه مشاكل مع سياسات الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="6f50c-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="6f50c-104">**المسألة:** نُهج الاستبقاء التي تم إنشاؤها حديثاً أو تحديثها في مركز إدارة Exchange لا يتم تطبيقها على علب البريد أو لا يتم نقل العناصر إلى علبة بريد الأرشيف أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="6f50c-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="6f50c-105">**الأسباب الجذرية:**</span><span class="sxs-lookup"><span data-stu-id="6f50c-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="6f50c-106">قد يكون هذا بسبب **"مساعد المجلد المدار"** لم تتم معالجة علبة البريد الخاصة بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="6f50c-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="6f50c-107">يحاول "مساعد المجلد المُدار" معالجة كل علبة بريد في المؤسسة المستندة إلى مجموعة النظراء مرة كل سبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="6f50c-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="6f50c-108">إذا قمت بتغيير علامة استبقاء أو تطبيق نهج استبقاء مختلف على علبة بريد، يمكنك الانتظار حتى معالجة "مساعدة المجلدات المدارة" علبة البريد، أو يمكنك تشغيل cmdlet Start-ManagedFolderAssistant لبدء "مساعد المجلدات المدارة" لمعالجة علبة بريد معينة.</span><span class="sxs-lookup"><span data-stu-id="6f50c-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="6f50c-109">إن تشغيل cmdlet هذا مفيد لاختبار أو استكشاف نهج استبقاء أو إعدادات علامة الاستبقاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="6f50c-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="6f50c-110">لمزيد من المعلومات، قم بزيارة [تشغيل مساعد المجلدات المدارة](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="6f50c-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="6f50c-111">**الحل:** تشغيل الأمر التالي لبدء تشغيل "مساعد المجلدات المدارة" لعلبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="6f50c-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="6f50c-112">قد يحدث هذا أيضًا إذا تم **تمكين** **استبقاء** على علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="6f50c-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="6f50c-113">إذا تم وضع علبة البريد على استبقاء، لن تتم معالجة نهج الاستبقاء على علبة البريد خلال ذلك الوقت.</span><span class="sxs-lookup"><span data-stu-id="6f50c-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="6f50c-114">لمزيد من المعلومات على إعداد الاحتفاظ انظر: [احتجاز الاحتفاظ علبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="6f50c-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="6f50c-115">**حل:**</span><span class="sxs-lookup"><span data-stu-id="6f50c-115">**Solution:**</span></span>
    
  - <span data-ttu-id="6f50c-116">تحقق من حالة إعداد الاحتفاظ على علبة البريد المحددة في [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="6f50c-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="6f50c-117">تشغيل الأمر التالي **لتعطيل** الاحتفاظ على علبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="6f50c-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="6f50c-118">الآن، إعادة تشغيل "مساعد المجلد المدارة":</span><span class="sxs-lookup"><span data-stu-id="6f50c-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="6f50c-119">**ملاحظة:** إذا كان علبة بريد أصغر من 10 ميغابايت، مساعد المجلدات المدارة لا تلقائياً معالجة علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="6f50c-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="6f50c-120">لمزيد من المعلومات حول نُهج الاستبقاء في مركز إدارة Exchange، راجع:</span><span class="sxs-lookup"><span data-stu-id="6f50c-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="6f50c-121">علامات الاستبقاء وسياسات الاستبقاء</span><span class="sxs-lookup"><span data-stu-id="6f50c-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="6f50c-122">تطبيق نهج استبقاء على علب البريد</span><span class="sxs-lookup"><span data-stu-id="6f50c-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="6f50c-123">إضافة علامات الاستبقاء أو إزالتها</span><span class="sxs-lookup"><span data-stu-id="6f50c-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="6f50c-124">كيفية تحديد نوع احتجاز وضع على علبة بريد</span><span class="sxs-lookup"><span data-stu-id="6f50c-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
