---
title: نقل رسائل البريد الإلكتروني إلى صندوق بريد الأرشيف
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 9af8a4d3ce72fd901ff2f3a1aae0654c7213dd7e
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46522758"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5e113-102">نقل البريد الإلكتروني إلى صندوق بريد الأرشيف</span><span class="sxs-lookup"><span data-stu-id="5e113-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="5e113-103">إذا كنت تريد منا تشغيل الشيكات التلقائية للإعدادات المذكورة أدناه، حدد زر العودة <- في الجزء العلوي من هذه الصفحة، ومن ثم أدخل عنوان البريد الإلكتروني للمستخدم الذي لديه مشاكل في نقل البريد الإلكتروني إلى صندوق بريد الأرشيف الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="5e113-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="5e113-104">تأكد من تمكين **علبة بريد أرشيف.**</span><span class="sxs-lookup"><span data-stu-id="5e113-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5e113-105">إذا لم يكن كذلك، استخدم الخطوات المذكورة في [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبة البريد الأرشيف.</span><span class="sxs-lookup"><span data-stu-id="5e113-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5e113-106">لأرشفة الرسائل تلقائيًا إلى صندوق بريد الأرشيف، يجب تعيين علامة الاحتفاظ مع إجراء **النقل إلى الأرشيف** **لتطبيقها تلقائيًا على علامة علبة البريد بأكملها (افتراضي).**</span><span class="sxs-lookup"><span data-stu-id="5e113-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5e113-107">استخدم الخطوات هنا لإنشاء العلامة: [وضع علامة الأرشفة الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5e113-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5e113-108">بعد ذلك، أضف علامة **الأرشيف** إلى نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="5e113-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5e113-109">في مركز مسؤول Exchange، اختر **نُهج الاستبقاء** > إضافة **علامة نقل إلى الأرشيف** إلى النهج > **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5e113-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5e113-110">الآن [تعيين نهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم معينة.</span><span class="sxs-lookup"><span data-stu-id="5e113-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5e113-111">سيتم تطبيق نفس النهج على كل من صندوق البريد **الأساسي** و **"الأرشيف".**</span><span class="sxs-lookup"><span data-stu-id="5e113-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5e113-112">قد يكون من الضروري فرض "مساعد المجلد المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة إلى علبة البريد الخاصة بالمستخدم.</span><span class="sxs-lookup"><span data-stu-id="5e113-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5e113-113">تشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلد المُدار" لعلبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="5e113-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5e113-114">بدء-مدارةمبدأاًمبدأاً -هوية<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5e113-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5e113-115">لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج الأرشفة والحذف لصناديق البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5e113-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  