---
title: مشاكل في تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833062"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="2d4db-102">تصحيح رسالة تطبيقات Microsoft 365 "عذرا، حساب آخر من مؤسستك قد تم بالفعل الدخول"</span><span class="sxs-lookup"><span data-stu-id="2d4db-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="2d4db-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="2d4db-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="2d4db-104">قم بإزالة كل حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **Access للعمل أو المدرسة.**</span><span class="sxs-lookup"><span data-stu-id="2d4db-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="2d4db-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="2d4db-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="2d4db-106">**ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="2d4db-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="2d4db-107">(على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="2d4db-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="2d4db-108">افتح تطبيق Office، واختر **تسجيل**  >  **الخروج من** حساب  >  **الملف**. ثم سجل الدخول باستخدام حساب مستخدم مع ترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="2d4db-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="2d4db-109">للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="2d4db-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="2d4db-110">بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="2d4db-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="2d4db-111">لمزيد من المعلومات، راجع ["عذرا، حساب](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)آخر من مؤسستك قد تم بالفعل في هذا الكمبيوتر" في Office .</span><span class="sxs-lookup"><span data-stu-id="2d4db-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>