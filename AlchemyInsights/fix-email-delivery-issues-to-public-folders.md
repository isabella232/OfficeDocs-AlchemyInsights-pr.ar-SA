---
title: إصلاح مشكلات تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكينها بالبريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e261fe60843555fa45927b0a6b36e1ccf79fb028
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716339"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="0dba5-102">إصلاح مشكلات تسليم البريد الإلكتروني إلى المجلدات العامة التي تم تمكينها بالبريد</span><span class="sxs-lookup"><span data-stu-id="0dba5-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="0dba5-103">إذا لم يتمكن المرسلون الخارجيون من إرسال رسائل إلى المجلدات العامة التي تم تمكينها بالبريد، وتلقى المرسلون الخطأ: **لا يمكن العثور عليها (550 5.4.1)،** فتحقق من تكوين مجال البريد الإلكتروني للمجلد العام كمجال ترحيل داخلي بدلاً من مجال موثوق به:</span><span class="sxs-lookup"><span data-stu-id="0dba5-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="0dba5-104">افتح [مركز إدارة Exchange (EAC).](https://docs.microsoft.com/Exchange/exchange-admin-center)</span><span class="sxs-lookup"><span data-stu-id="0dba5-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="0dba5-105">انتقل إلى \> **المجالات المقبولة لتدفق** **البريد،** وحدد المجال المقبول، ثم انقر فوق **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="0dba5-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="0dba5-106">في صفحة الخصائص التي تفتح، إذا تم تعيين نوع المجال إلى **"موثوق"،** قم بتغيير القيمة إلى **الترحيل الداخلي** ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="0dba5-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="0dba5-107">إذا تلقى المرسلون الخارجيون الخطأ **ليس لديك إذن (550 5.7.13)**، قم بتشغيل الأمر التالي في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) لرؤية الأذونات للمستخدمين المجهولين في المجلد العمومي:</span><span class="sxs-lookup"><span data-stu-id="0dba5-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="0dba5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`على سبيل `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`المثال، .</span><span class="sxs-lookup"><span data-stu-id="0dba5-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="0dba5-109">للسماح للمستخدمين الخارجيين بإرسال بريد إلكتروني إلى هذا المجلد العام، أضف حق الوصول إلى CreateItems إلى المستخدم Anonymous.</span><span class="sxs-lookup"><span data-stu-id="0dba5-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="0dba5-110">على سبيل `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`المثال، .</span><span class="sxs-lookup"><span data-stu-id="0dba5-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
