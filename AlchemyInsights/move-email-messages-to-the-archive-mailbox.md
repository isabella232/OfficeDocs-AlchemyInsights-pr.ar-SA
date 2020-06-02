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
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511027"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5886e-102">نقل البريد الإلكتروني إلى صندوق بريد الأرشيف</span><span class="sxs-lookup"><span data-stu-id="5886e-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="5886e-103">تأكد من تمكين **علبة بريد أرشيف.**</span><span class="sxs-lookup"><span data-stu-id="5886e-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5886e-104">إذا لم يكن كذلك، استخدم الخطوات في [هذه المقالة](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) لتمكين علبة بريد الأرشيف.</span><span class="sxs-lookup"><span data-stu-id="5886e-104">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5886e-105">لأرشفة الرسائل تلقائيًا إلى صندوق بريد الأرشيف، يجب تعيين علامة الاحتفاظ مع إجراء **النقل إلى الأرشيف** ليتم تطبيقها **تلقائيًا على علامة علبة البريد بأكملها (الافتراضية).**</span><span class="sxs-lookup"><span data-stu-id="5886e-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5886e-106">استخدم الخطوات هنا لإنشاء العلامة: [علامة الأرشيف الافتراضية](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5886e-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5886e-107">بعد ذلك، أضف علامة **الأرشيف** إلى سياسة الاحتفاظ.</span><span class="sxs-lookup"><span data-stu-id="5886e-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5886e-108">في مركز إدارة Exchange، اختر **نُهج الاحتفاظ** > إضافة **علامة الانتقال إلى الأرشيف** إلى النهج > **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5886e-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5886e-109">الآن [تعيين نهج الاحتفاظ](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم معينة.</span><span class="sxs-lookup"><span data-stu-id="5886e-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5886e-110">سيتم تطبيق نفس النهج على كل من **علبة** البريد الأساسية **وعلبة البريد الأرشيف.**</span><span class="sxs-lookup"><span data-stu-id="5886e-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5886e-111">قد يكون من الضروري فرض "مساعد المجلد المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة على علبة بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="5886e-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5886e-112">تشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلد المدار" لعلبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="5886e-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5886e-113">بدء إدارة FolderedAssistant -الهوية<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5886e-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5886e-114">لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج أرشيف وحذف لصناديق البريد](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5886e-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  