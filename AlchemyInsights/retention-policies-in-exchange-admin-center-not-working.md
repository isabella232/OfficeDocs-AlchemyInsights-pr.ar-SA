---
title: لا تعمل سياسات الاستبقاء في مركز إدارة Exchange
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
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952215"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="ca525-102">سياسات الاستبقاء في مركز إدارة Exchange</span><span class="sxs-lookup"><span data-stu-id="ca525-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="ca525-103">إذا كنت تريد منا تشغيل عمليات التحقق التلقائية من الإعدادات المذكورة أدناه، فحدد زر الخلف <-- في أعلى هذه الصفحة، ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي يواجه مشاكل في سياسات الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="ca525-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="ca525-104">إذا كنت تواجه مشاكل مع سياسات الاستبقاء في مركز إدارة Exchange التي لا تنطبق على علب البريد أو العناصر التي لا تنتقل إلى علبة بريد الأرشيف، فتحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="ca525-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="ca525-105">**الأسباب الجذرية:**</span><span class="sxs-lookup"><span data-stu-id="ca525-105">**Root Causes:**</span></span>

- <span data-ttu-id="ca525-106">**لم يعالج "مساعد** المجلد المدار" علبة بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="ca525-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="ca525-107">يحاول مساعد المجلد المدار معالجة كل علبة بريد في مؤسستك المستندة إلى السحابة مرة واحدة كل سبعة أيام.</span><span class="sxs-lookup"><span data-stu-id="ca525-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="ca525-108">**الحل:** تشغيل مساعد المجلد المدار.</span><span class="sxs-lookup"><span data-stu-id="ca525-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="ca525-109">**تم تمكين RetentionHold** **على** علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="ca525-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="ca525-110">إذا تم وضع علبة البريد على RetentionHold، لن تتم معالجة نهج الاستبقاء على علبة البريد خلال هذه الفترة.</span><span class="sxs-lookup"><span data-stu-id="ca525-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="ca525-111">**الحل:** تحقق من حالة إعداد "احتجاز الاستبقاء" والتحديث حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="ca525-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="ca525-112">للحصول على التفاصيل، راجع [الاستمرار في استبقاء علبة البريد](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="ca525-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="ca525-113">**ملاحظة:** إذا كانت علبة البريد أصغر من 10 مبايت، فإن مساعد المجلد المدار لن يقوم تلقائيا لمعالجة علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="ca525-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="ca525-114">لمزيد من المعلومات حول سياسات الاستبقاء في مركز إدارة Exchange، راجع:</span><span class="sxs-lookup"><span data-stu-id="ca525-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="ca525-115">علامات الاستبقاء ونهج الاستبقاء</span><span class="sxs-lookup"><span data-stu-id="ca525-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="ca525-116">[تطبيق نهج استبقاء على علب](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) البريد أو [إضافة علامات استبقاء أو إزالتها](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="ca525-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="ca525-117">كيفية تحديد نوع الانتظار الموضوع على علبة بريد</span><span class="sxs-lookup"><span data-stu-id="ca525-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
