---
title: إصلاح مشاكل التسليم الإلكتروني للمجلدات العمومية التي تعتمد البريد
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.assetid: ''
ms.openlocfilehash: e24a4db2deb3f691209a1634d932ed277a79c868
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35387692"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="22d27-102">إصلاح مشاكل التسليم الإلكتروني للمجلدات العمومية التي تعتمد البريد</span><span class="sxs-lookup"><span data-stu-id="22d27-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="22d27-103">إذا لم يكن المرسلين الخارجيين لا يمكن إرسال الرسائل إلى المجلدات العمومية التي تعتمد البريد ومرسلي رسالة الخطأ: **تعذر العثور على (550 5.4.1)**، تحقق من مجال بريد إلكتروني للمجلد العمومي تم تكوينه كمجال ترحيل داخلي بدلاً من المجال الموثوق:</span><span class="sxs-lookup"><span data-stu-id="22d27-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="22d27-104">فتح [مركز مسؤول Exchange (شرق)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="22d27-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="22d27-105">انتقل إلى **تدفق البريد** \> **مجالات مقبولة**، حدد المجال المقبول، وثم انقر فوق **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="22d27-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="22d27-106">في الخصائص ذلك الفتح الصفحة إذا تم تعيين نوع المجال إلى **حجية**وتغيير القيمة إلى **ترحيل داخلي** وثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="22d27-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="22d27-107">في حالة ظهور المرسلين الخارجيين الخطأ **ليس لديك الإذن (550 5.7.13)**، تشغيل الأمر التالي في [PowerShell Exchange عبر إنترنت](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) لعرض الأذونات للمستخدمين المجهولين في المجلد العمومي:</span><span class="sxs-lookup"><span data-stu-id="22d27-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="22d27-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`على سبيل المثال، `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="22d27-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="22d27-109">للسماح للمستخدمين الخارجيين بإرسال بريد إلكتروني إلى هذا المجلد العمومي، إضافة الوصول كريتيتيمس اليمين للمستخدم المجهول.</span><span class="sxs-lookup"><span data-stu-id="22d27-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="22d27-110">على سبيل المثال، `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="22d27-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>
