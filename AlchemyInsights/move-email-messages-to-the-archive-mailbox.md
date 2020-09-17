---
title: نقل رسائل البريد الكتروني إلى علبه بريد الأرشيف
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
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799767"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="fc3cb-102">نقل البريد الكتروني إلى علبه بريد الأرشيف</span><span class="sxs-lookup"><span data-stu-id="fc3cb-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="fc3cb-103">إذا كنت تريد ان يقومنا بتشغيل التدقيق التلقائي للإعدادات المذكورة أدناه ، فحدد الزر السابق < وفي اعلي هذه الصفحة ، ثم ادخل عنوان البريد الكتروني للمستخدم الذي لديه مشاكل في نقل البريد الكتروني إلى علبه بريد الأرشيف الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="fc3cb-104">تاكد من تمكين **علبه بريد الأرشيف** .</span><span class="sxs-lookup"><span data-stu-id="fc3cb-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="fc3cb-105">إذا لم يكن كذلك ، فاستخدم الخطوات [المذكورة في هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبه بريد الأرشيف.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="fc3cb-106">لأرشفه الرسائل تلقائيا إلى علبه بريد الأرشيف ، يجب تعيين علامة الاستبقاء التي تحتوي علي الاجراء **نقل إلى الارشفه** **تلقائيا إلى الوضع "التطبيق" علي علبه البريد بالبالكامل (افتراضي)**.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="fc3cb-107">استخدم الخطوات الواردة هنا لإنشاء العلامة: [أرشفه العلامة الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="fc3cb-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="fc3cb-108">بعد ذلك ، أضف علامة **الأرشيف** إلى نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="fc3cb-109">في مركز أداره Exchange ، اختر **نهج الاستبقاء** > أضف **علامة النقل إلى الأرشيف** إلى النهج ال> **حفظه**.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="fc3cb-110">[الآن يمكنك تعيين نهج الاستبقاء](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبه البريد الخاصة بالمستخدم المحدد.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="fc3cb-111">سيتم تطبيق نفس النهج علي كل من علبه البريد **الاساسيه** **والارشفه** .</span><span class="sxs-lookup"><span data-stu-id="fc3cb-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="fc3cb-112">قد يكون من الضروري فرض مساعد المجلد المدار (MFA) لتشغيل الإعدادات الجديدة وتطبيقها علي علبه بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="fc3cb-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="fc3cb-113">قم بتشغيل الأمر التالي اثناء [الاتصال ب أكسو PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل مساعد المجلد المدار لعلبه بريد معينه:</span><span class="sxs-lookup"><span data-stu-id="fc3cb-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="fc3cb-114">بدء الماناجيدفولديراسيستانت-الهوية <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="fc3cb-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="fc3cb-115">للحصول علي مزيد من المعلومات حول اعداد نهج أرشفه ، راجع اعداد [نهج الارشفه والحذف لعلب البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="fc3cb-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  