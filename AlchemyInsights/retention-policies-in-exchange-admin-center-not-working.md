---
title: نهج الاستبقاء في مركز أداره Exchange لا تعمل
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 1fee2361b2dd6e0989d430a17aebb13bd5948578
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740497"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="d1479-102">نهج الاستبقاء في مركز أداره Exchange</span><span class="sxs-lookup"><span data-stu-id="d1479-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="d1479-103">إذا كنت تريد ان نقوم بتشغيل التدقيق التلقائي للإعدادات المذكورة أدناه ، فحدد الزر السابق <--في اعلي هذه الصفحة ، ثم ادخل عنوان البريد الكتروني الخاص بالمستخدم الذي لديه مشاكل في نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="d1479-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

 <span data-ttu-id="d1479-104">**المشكلة:** لا يتم تطبيق نهج الاستبقاء التي تم إنشاؤها أو تحديثها حديثا في "مركز أداره Exchange" علي علب البريد أو العناصر التي لا يتم نقلها إلى علبه بريد الأرشيف أو حذفها.</span><span class="sxs-lookup"><span data-stu-id="d1479-104">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="d1479-105">**الأسباب الاساسيه:**</span><span class="sxs-lookup"><span data-stu-id="d1479-105">**Root Causes:**</span></span>
  
- <span data-ttu-id="d1479-106">قد يعود سبب ذلك إلى عدم قيام **مساعد المجلد المدار** بمعالجه علبه بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="d1479-106">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="d1479-107">يحاول مساعد المجلد المدار معالجه كل علبه بريد في المؤسسة المستندة إلى السحابة مره واحده كل سبعه أيام.</span><span class="sxs-lookup"><span data-stu-id="d1479-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="d1479-108">إذا قمت بتغيير علامة استبقاء أو تطبيق نهج استبقاء مختلف علي علبه بريد ، فيمكنك الانتظار حتى يقوم المجلد المدار بمعالجه علبه البريد ، أو يمكنك تشغيل الأمر ماناجيدفولديراسيستانت cmdlet لبدء تشغيل "مساعد المجلد المدار" لمعالجه علبه بريد معينه.</span><span class="sxs-lookup"><span data-stu-id="d1479-108">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="d1479-109">يعتبر تشغيل أمر cmdlet هذا مفيدا لاختبار إعدادات نهج الاستبقاء أو علامة الاستبقاء أو استكشاف الأخطاء فيها.</span><span class="sxs-lookup"><span data-stu-id="d1479-109">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="d1479-110">لمزيد من المعلومات ، قم بزيارة [تشغيل مساعد المجلد المدار](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="d1479-110">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="d1479-111">**الحل:** قم بتشغيل الأمر التالي لبدء تشغيل مساعد المجلد المدار لعلبه بريد معينه:</span><span class="sxs-lookup"><span data-stu-id="d1479-111">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="d1479-112">قد يحدث هذا أيضا إذا تم **تمكين** **ريتينتيونهولد** علي علبه البريد.</span><span class="sxs-lookup"><span data-stu-id="d1479-112">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="d1479-113">إذا تم وضع علبه البريد علي ريتينتيونهولد ، فلن تتم معالجه نهج الاستبقاء علي علبه البريد خلال هذا الوقت.</span><span class="sxs-lookup"><span data-stu-id="d1479-113">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="d1479-114">للحصول علي مزيد من الإينفورماتون علي اعداد ريتينتيونهولد ، راجع: [احتجاز استبقاء علبه البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="d1479-114">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="d1479-115">**Solution**</span><span class="sxs-lookup"><span data-stu-id="d1479-115">**Solution:**</span></span>
    
  - <span data-ttu-id="d1479-116">تحقق من حاله اعداد ريتينتيونهولد علي علبه البريد المحددة في [أكسو powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span><span class="sxs-lookup"><span data-stu-id="d1479-116">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="d1479-117">قم بتشغيل الأمر التالي **لتعطيل** ريتينتيونهولد علي علبه بريد معينه:</span><span class="sxs-lookup"><span data-stu-id="d1479-117">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="d1479-118">الآن ، أعد تشغيل مساعد المجلدات المدارة:</span><span class="sxs-lookup"><span data-stu-id="d1479-118">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="d1479-119">**ملاحظه:** إذا كانت علبه البريد أصغر من 10 ميغابايت ، فلن يعالج مساعد المجلد المدار علبه البريد تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="d1479-119">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="d1479-120">للحصول علي مزيد من المعلومات حول نهج الاستبقاء في مركز أداره Exchange ، راجع:</span><span class="sxs-lookup"><span data-stu-id="d1479-120">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="d1479-121">علامات الاستبقاء ونهج الاستبقاء</span><span class="sxs-lookup"><span data-stu-id="d1479-121">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="d1479-122">تطبيق نهج استبقاء علي علب البريد</span><span class="sxs-lookup"><span data-stu-id="d1479-122">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="d1479-123">أضافه علامات الاستبقاء أو ازالتها</span><span class="sxs-lookup"><span data-stu-id="d1479-123">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="d1479-124">كيفيه تحديد نوع التعليق الموضوع علي علبه بريد</span><span class="sxs-lookup"><span data-stu-id="d1479-124">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
