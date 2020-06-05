---
title: مشكلات تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: e4f2fea5c2f368ae240614ee1f7bc729338dd75d
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579924"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="245c1-102">إصلاح تطبيقات Microsoft 365 "عذراً، تم تسجيل الدخول بالفعل لحساب آخر من مؤسستك"</span><span class="sxs-lookup"><span data-stu-id="245c1-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="245c1-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="245c1-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="245c1-104">قم بإزالة كافة حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **الوصول إلى العمل أو المدرسة**.</span><span class="sxs-lookup"><span data-stu-id="245c1-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="245c1-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="245c1-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="245c1-106">**ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="245c1-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="245c1-107">(على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="245c1-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="245c1-108">افتح تطبيق Office، اختر تسجيل الخروج من حساب **الملف**  >  **Account**  >  **Sign Out**. ثم قم بتسجيل الدخول باستخدام حساب مستخدم بترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="245c1-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="245c1-109">للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="245c1-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="245c1-110">بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="245c1-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="245c1-111">لمزيد من المعلومات، راجع ["عذراً، تم تسجيل الدخول بالفعل لحساب آخر من مؤسستك على هذا الكمبيوتر" في Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="245c1-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>