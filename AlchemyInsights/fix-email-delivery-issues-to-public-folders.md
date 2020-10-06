---
title: إصلاح مشاكل تسليم البريد الكتروني إلى المجلدات العمومية الممكنة للبريد
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
- "1956"
- "3500007"
ms.openlocfilehash: 74a26306766ed7952a3bbbcb06f1f0113a113024
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366451"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="7e7c9-102">إصلاح مشاكل تسليم البريد الكتروني إلى المجلدات العمومية الممكنة للبريد</span><span class="sxs-lookup"><span data-stu-id="7e7c9-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="7e7c9-103">إذا تعذر علي المرسلين الخارجيين إرسال رسائل إلى المجلدات العمومية الممكنة للبريد الكتروني ، وتلقي المرسلين الخطا: **تعذر العثور عليه (550 5.4.1)**، تاكد من تكوين مجال البريد الكتروني للمجلد العمومي كمجال الترحيل الداخلي بدلا من مجال موثوق به:</span><span class="sxs-lookup"><span data-stu-id="7e7c9-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="7e7c9-104">فتح [مركز أداره Exchange (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="7e7c9-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="7e7c9-105">انتقل إلى **Mail flow** \> **المجالات المقبولة**لتدفق البريد ، وحدد المجال المقبول ، ثم انقر فوق **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="7e7c9-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="7e7c9-106">في صفحه الخصائص التي يتم فتحها ، إذا تم تعيين نوع المجال إلى **مخول**، فقم بتغيير القيمة إلى **الترحيل الداخلي** ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="7e7c9-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="7e7c9-107">إذا تلقي المرسلون الخارجيون الخطا **(550 5.7.13)**، فقم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) للاطلاع علي الأذونات الخاصة بالمستخدمين المجهولين في المجلد العام:</span><span class="sxs-lookup"><span data-stu-id="7e7c9-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="7e7c9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` علي سبيل المثال ، `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous` .</span><span class="sxs-lookup"><span data-stu-id="7e7c9-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="7e7c9-109">للسماح للمستخدمين الخارجيين بإرسال البريد الكتروني إلى هذا المجلد العام ، أضف حق وصول كرياتيتيمس إلى المستخدم مجهول.</span><span class="sxs-lookup"><span data-stu-id="7e7c9-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="7e7c9-110">علي سبيل المثال ، `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems` .</span><span class="sxs-lookup"><span data-stu-id="7e7c9-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
