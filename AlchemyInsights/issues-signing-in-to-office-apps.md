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
- "2560"
ms.openlocfilehash: de0a1b78724db9a8e93d8d599ce3b503abcb86e2
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938117"
---
# <a name="fixing-the-office-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="24f08-102">تحديد رسالة "عفوا، الدخول حساب آخر من الشركة الخاصة بك بالفعل" تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="24f08-102">Fixing the Office apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="24f08-103">لإصلاح هذا الخطأ، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="24f08-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="24f08-104">قم بإزالة كافة حسابات العمل إلا على حساب المتأثرة، واستخدام > إعدادات Windows **الوصول إلى العمل أو المدرسة**.</span><span class="sxs-lookup"><span data-stu-id="24f08-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="24f08-105">["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="24f08-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="24f08-106">**ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="24f08-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="24f08-107">(مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="24f08-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="24f08-108">فتح تطبيق Office، اختر **ملف** > **حساب** > **تسجيل الخروج**. قم بتسجيل الدخول باستخدام حساب مستخدم لديه ترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="24f08-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="24f08-109">للحصول على معلومات مفصلة، راجع [الحسابات في المكتب](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="24f08-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="24f08-110">لنظام التشغيل Mac، راجع [إمكانية تسجيل الدخول إلى 2016 Office للتطبيق Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="24f08-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="24f08-111">لمزيد من المعلومات، راجع ["عفوا، حساب آخر من الشركة الخاصة بك يتم تسجيل الدخول بالفعل على هذا الكمبيوتر" في مكتب](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="24f08-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>