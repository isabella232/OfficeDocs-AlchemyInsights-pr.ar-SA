---
title: نقل رسائل البريد الإلكتروني إلى علبة بريد الأرشيف
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 5592bc7d4566e3498c33bbf9488db7f46ec58842
ms.sourcegitcommit: 8864b5789d9905916039081b53530c7e6d8bc529
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/10/2019
ms.locfileid: "36822149"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="5b7b7-102">نقل البريد الإلكتروني إلى صندوق بريد الأرشيف</span><span class="sxs-lookup"><span data-stu-id="5b7b7-102">Move email to the archive mailbox</span></span>

1. <span data-ttu-id="5b7b7-103">تأكد من تمكين **علبة بريد أرشيف.**</span><span class="sxs-lookup"><span data-stu-id="5b7b7-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="5b7b7-104">إذا لم يكن الأمر كذلك، اتبع الخطوات المذكورة في [هذه المقالة](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة بريد الأرشيف.</span><span class="sxs-lookup"><span data-stu-id="5b7b7-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="5b7b7-105">لأرشفة الرسائل تلقائيًا إلى علبة بريد الأرشيف، يجب تعيين علامة استبقاء مع إجراء **النقل إلى الأرشيف** ليتم **تطبيقها تلقائيًا على علامة علبة البريد بأكملها (افتراضية).**</span><span class="sxs-lookup"><span data-stu-id="5b7b7-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="5b7b7-106">استخدم الخطوات هنا لإنشاء العلامة: [أرشفة العلامة الافتراضية](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span><span class="sxs-lookup"><span data-stu-id="5b7b7-106">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="5b7b7-107">بعد ذلك، أضف علامة **الأرشيف** إلى نهج الاستبقاء.</span><span class="sxs-lookup"><span data-stu-id="5b7b7-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="5b7b7-108">في مركز مسؤول Exchange، اختر **نُهج الاستبقاء** > إضافة **علامة نقل إلى الأرشيف** إلى النهج > **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="5b7b7-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="5b7b7-109">الآن [تعيين "نهج الاستبقاء"](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) إلى علبة بريد المستخدم المحدد.</span><span class="sxs-lookup"><span data-stu-id="5b7b7-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="5b7b7-110">سيتم تطبيق نفس النهج على كل من علبة البريد **الأساسية** **والأرشيف.**</span><span class="sxs-lookup"><span data-stu-id="5b7b7-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="5b7b7-111">قد يكون من الضروري فرض "مساعد المجلدات المدارة" (MFA) لتشغيل وتطبيق الإعدادات الجديدة على علبة بريد المستخدم.</span><span class="sxs-lookup"><span data-stu-id="5b7b7-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="5b7b7-112">قم بتشغيل الأمر التالي أثناء [الاتصال بـ EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء تشغيل "مساعد المجلدات المدارة" لعلبة بريد معينة:</span><span class="sxs-lookup"><span data-stu-id="5b7b7-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="5b7b7-113">بدء مُدارفولديرمساعد-الهوية<name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="5b7b7-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="5b7b7-114">لمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج أرشفة وحذف لعلب البريد](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="5b7b7-114">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  