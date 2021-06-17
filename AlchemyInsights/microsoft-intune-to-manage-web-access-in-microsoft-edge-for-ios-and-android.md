---
title: استخدام Microsoft Intune لإدارة الوصول إلى الويب في Microsoft Edge لنظامي التشغيل iOS وAndroid
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003846"
- "6895"
- "9006502"
- "11144"
ms.openlocfilehash: a6c6f9563933b7cf6b71c4758c29ffd94617c4be
ms.sourcegitcommit: 7a406a3d4680662e81f0056454f7e25fb2f52504
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/17/2021
ms.locfileid: "52989636"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="c429a-102">استخدام Microsoft Intune لإدارة الوصول إلى الويب في Microsoft Edge لنظامي التشغيل iOS وAndroid</span><span class="sxs-lookup"><span data-stu-id="c429a-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="c429a-103">يتيح Microsoft Edge لنظامي التشغيل iOS وAndroid للمستخدم استعراض الويب من ملفات تعريف متعددة منفصلة تماما.</span><span class="sxs-lookup"><span data-stu-id="c429a-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="c429a-104">تتوفر إمكانات الحماية الأكبر لبيانات Microsoft 365 عند الاشتراك في مجموعة Enterprise Mobility + Security، التي تتضمن ميزات Microsoft Intune و Azure Active Directory Premium، مثل الوصول الشرطي.</span><span class="sxs-lookup"><span data-stu-id="c429a-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="c429a-105">على الأقل، سترغب في نشر نهج وصول شرطي يسمح (1) للمستخدمين بالاتصال من الأجهزة المحمولة ب Microsoft Edge لنظامي التشغيل iOS وAndroid، وذلك (2) بتنفيذ نهج حماية تطبيق Microsoft Intune الذي يوفر تجربة استعراض محمية.</span><span class="sxs-lookup"><span data-stu-id="c429a-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="c429a-106">لفهم كيفية استخدام الوصول الشرطي ونهجه، راجع:</span><span class="sxs-lookup"><span data-stu-id="c429a-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="c429a-107">تطبيق سياسات الوصول الشرطي في Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="c429a-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="c429a-108">إنشاء سياسات حماية تطبيق Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c429a-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="c429a-109">استخدام تسجيل الدخول المفرد لتطبيقات الويب المتصلة ب Azure Active Directory في المستعرضات المحمية ب النهج</span><span class="sxs-lookup"><span data-stu-id="c429a-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="c429a-110">استخدام تكوين التطبيق لإدارة تجربة الاستعراض</span><span class="sxs-lookup"><span data-stu-id="c429a-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="c429a-111">السماح باستخدام حسابات العمل والمدرسة فقط</span><span class="sxs-lookup"><span data-stu-id="c429a-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="c429a-112">نشر سياسات تكوين التطبيق العامة</span><span class="sxs-lookup"><span data-stu-id="c429a-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="c429a-113">نشر سياسات تكوين التطبيق لحماية البيانات</span><span class="sxs-lookup"><span data-stu-id="c429a-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="c429a-114">استخدام Microsoft Endpoint Manager لنشر سياسات تكوين التطبيق</span><span class="sxs-lookup"><span data-stu-id="c429a-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="c429a-115">للتعرف على كيفية الوصول إلى سجلات التطبيقات المدارة، راجع [استخدام Microsoft Edge لنظامي التشغيل iOS](https://go.microsoft.com/fwlink/?linkid=2132578)وAndroid للوصول إلى سجلات التطبيقات المدارة .</span><span class="sxs-lookup"><span data-stu-id="c429a-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
