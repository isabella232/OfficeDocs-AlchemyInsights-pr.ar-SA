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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938118"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="11e32-102">مشكلات تسجيل الدخول إلى تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="11e32-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="11e32-103">لإصلاح مشكلات تسجيل الدخول مع تطبيقات Office، قم ما يلي:</span><span class="sxs-lookup"><span data-stu-id="11e32-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="11e32-104">قم بإزالة كافة حسابات العمل إلا على حساب المتأثرة، واستخدام > إعدادات Windows **الوصول إلى العمل أو المدرسة**.</span><span class="sxs-lookup"><span data-stu-id="11e32-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="11e32-105">["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="11e32-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="11e32-106">**ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="11e32-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="11e32-107">(مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="11e32-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="11e32-108">فتح تطبيق Office، اختر **ملف** > **حساب** > **تسجيل الخروج**. قم بتسجيل الدخول باستخدام حساب مستخدم لديه ترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="11e32-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="11e32-109">للحصول على معلومات مفصلة، راجع [الحسابات في المكتب](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="11e32-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="11e32-110">لنظام التشغيل Mac، راجع [إمكانية تسجيل الدخول إلى 2016 Office للتطبيق Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="11e32-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="11e32-111">في حالة حدوث الأخطاء أثناء الاتصال باستخدام Office 2013 Office 365، تمكين مصادقة عميل Office الحديثة.</span><span class="sxs-lookup"><span data-stu-id="11e32-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="11e32-112">للحصول على مزيد من المعلومات، راجع:</span><span class="sxs-lookup"><span data-stu-id="11e32-112">For more information, see:</span></span>
- [<span data-ttu-id="11e32-113">لا يمكنك تسجيل الدخول إلى Office 365 أو Azure إينتوني</span><span class="sxs-lookup"><span data-stu-id="11e32-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="11e32-114">مشكلات الاتصال في تسجيل الدخول بعد التحديث إلى عام 2016 Office بناء 16.0.7967 على Windows 10</span><span class="sxs-lookup"><span data-stu-id="11e32-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="11e32-115">"عفوا، حساب آخر من الشركة الخاصة بك يتم تسجيل الدخول بالفعل على هذا الكمبيوتر" في Office</span><span class="sxs-lookup"><span data-stu-id="11e32-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="11e32-116">استكشاف مشكلات تسجيل الدخول بمصادقة الحديثة Office عند استخدام ADFS</span><span class="sxs-lookup"><span data-stu-id="11e32-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)