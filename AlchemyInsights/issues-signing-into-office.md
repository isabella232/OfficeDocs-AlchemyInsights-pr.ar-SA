---
title: مشكلات تسجيل الدخول إلى تطبيقات Office
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
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43762962"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="810bb-102">مشكلات تسجيل الدخول إلى تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="810bb-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="810bb-103">لإصلاح مشكلات تسجيل الدخول مع تطبيقات Office، جرّب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="810bb-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="810bb-104">قم بإزالة كافة حسابات العمل، باستثناء الحساب المتأثر، باستخدام إعدادات Windows > **الوصول إلى العمل أو المدرسة**.</span><span class="sxs-lookup"><span data-stu-id="810bb-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="810bb-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="810bb-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="810bb-106">**ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="810bb-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="810bb-107">(على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="810bb-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="810bb-108">افتح تطبيق Office، اختر**تسجيل الخروج\*\*\*\*من حساب** >  **الملف** > . ثم قم بتسجيل الدخول باستخدام حساب مستخدم بترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="810bb-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="810bb-109">للحصول على معلومات مفصلة، راجع [حسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="810bb-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="810bb-110">بالنسبة لأجهزة Mac، راجع [يتعذر عليك تسجيل الدخول إلى تطبيق Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="810bb-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="810bb-111">إذا حدثت الأخطاء أثناء الاتصال بـ Microsoft 365 باستخدام Office 2013، قم بتمكين المصادقة الحديثة لعميل Office.</span><span class="sxs-lookup"><span data-stu-id="810bb-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="810bb-112">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="810bb-112">For more information, see:</span></span>
- [<span data-ttu-id="810bb-113">لا يمكنك تسجيل الدخول إلى Microsoft 365 أو Azure أو Intune</span><span class="sxs-lookup"><span data-stu-id="810bb-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="810bb-114">مشكلات الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 إنشاء 16.0.7967 على Windows 10</span><span class="sxs-lookup"><span data-stu-id="810bb-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="810bb-115">"عذراً، تم تسجيل الدخول بالفعل إلى حساب آخر من مؤسستك على هذا الكمبيوتر" في Office</span><span class="sxs-lookup"><span data-stu-id="810bb-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="810bb-116">استكشاف مشكلات تسجيل الدخول وإصلاحها باستخدام مصادقة Office الحديثة عند استخدام ADFS</span><span class="sxs-lookup"><span data-stu-id="810bb-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)