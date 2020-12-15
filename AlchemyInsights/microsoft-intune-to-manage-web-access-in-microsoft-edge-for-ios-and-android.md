---
title: استخدام Microsoft Intune لأداره الوصول إلى الويب في Microsoft Edge ل iOS و Android
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
ms.openlocfilehash: 4d6ab4df4ff9588ce5052421602e347c76c91c3f
ms.sourcegitcommit: a7952283882d341515623d5ae58eda14d0553449
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/10/2020
ms.locfileid: "49676773"
---
# <a name="use-microsoft-intune-to-manage-web-access-in-microsoft-edge-for-ios-and-android"></a><span data-ttu-id="04a80-102">استخدام Microsoft Intune لأداره الوصول إلى الويب في Microsoft Edge ل iOS و Android</span><span class="sxs-lookup"><span data-stu-id="04a80-102">Use Microsoft Intune to manage web access in Microsoft Edge for iOS and Android</span></span>

<span data-ttu-id="04a80-103">يسمح Microsoft Edge ل iOS و Android لمستخدم باستعراض الويب من العديد من ملفات التعريف المنفصلة بالبالكامل.</span><span class="sxs-lookup"><span data-stu-id="04a80-103">Microsoft Edge for iOS and Android lets a user browse the web from multiple, completely separate profiles.</span></span>

<span data-ttu-id="04a80-104">تتوفر قدرات الحماية الأكبر لبيانات Microsoft 365 عند الاشتراك في التنقل عبر المؤسسة + مجموعه الأمان ، التي تتضمن ميزات Microsoft Intune و Azure Active directory Premium ، مثل الوصول المشروط.</span><span class="sxs-lookup"><span data-stu-id="04a80-104">The broadest protection capabilities for Microsoft 365 data become available when you subscribe to the Enterprise Mobility + Security suite, which includes Microsoft Intune and Azure Active Directory Premium features, such as conditional access.</span></span> <span data-ttu-id="04a80-105">بحد ادني ، ستحتاج إلى نشر نهج وصول مشروط (1) يسمح للمستخدمين بالاتصال من الاجهزه المحمولة ب Microsoft Edge ل iOS و Android وانه (2) يطبق نهج حماية تطبيق Microsoft Intune الذي يوفر تجربه استعراض محمية.</span><span class="sxs-lookup"><span data-stu-id="04a80-105">At a minimum, you’ll want to deploy a conditional access policy that (1) lets users connect from mobile devices to Microsoft Edge for iOS and Android and that (2) implements a Microsoft Intune app-protection policy that provides a protected browsing experience.</span></span>

<span data-ttu-id="04a80-106">لفهم كيف يمكنك استخدام الوصول الشرطي والنهج ، راجع:</span><span class="sxs-lookup"><span data-stu-id="04a80-106">To understand how you can use conditional access and policies, see:</span></span>

[<span data-ttu-id="04a80-107">تطبيق نهج الوصول المشروط ل Azure Active directory</span><span class="sxs-lookup"><span data-stu-id="04a80-107">Apply Azure Active Directory conditional access policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132481)

[<span data-ttu-id="04a80-108">إنشاء نهج حماية تطبيق Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="04a80-108">Create Microsoft Intune app protection policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132651)

[<span data-ttu-id="04a80-109">استخدام تسجيل الدخول الأحادي ل Azure Active directory-تطبيقات ويب متصلة في مستعرضات محمية بالنهج</span><span class="sxs-lookup"><span data-stu-id="04a80-109">Use single sign-on for Azure Active Directory–connected web apps in policy-protected browsers</span></span>](https://go.microsoft.com/fwlink/?linkid=2132482)

[<span data-ttu-id="04a80-110">استخدام تكوين التطبيق لأداره تجربه الاستعراض</span><span class="sxs-lookup"><span data-stu-id="04a80-110">Use app configuration to manage the browsing experience</span></span>](https://go.microsoft.com/fwlink/?linkid=2132483)

[<span data-ttu-id="04a80-111">السماح باستخدام حسابات العمل والمدرسة فقط</span><span class="sxs-lookup"><span data-stu-id="04a80-111">Allow the use of only work and school accounts</span></span>](https://go.microsoft.com/fwlink/?linkid=2132652)

[<span data-ttu-id="04a80-112">نشر نهج تكوين التطبيقات العامة</span><span class="sxs-lookup"><span data-stu-id="04a80-112">Deploy general app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132653)

[<span data-ttu-id="04a80-113">نشر نهج تكوين التطبيق لحماية البيانات</span><span class="sxs-lookup"><span data-stu-id="04a80-113">Deploy app configuration policies for data protection</span></span>](https://go.microsoft.com/fwlink/?linkid=2132654)

[<span data-ttu-id="04a80-114">استخدام Microsoft Endpoint Manager لنشر نهج تكوين التطبيق</span><span class="sxs-lookup"><span data-stu-id="04a80-114">Use Microsoft Endpoint Manager to deploy app configuration policies</span></span>](https://go.microsoft.com/fwlink/?linkid=2132707)

<span data-ttu-id="04a80-115">للتعرف علي كيفيه الوصول إلى سجلات التطبيقات المدارة ، راجع [استخدام Microsoft Edge ل iOS و Android للوصول إلى سجلات التطبيقات المدارة](https://go.microsoft.com/fwlink/?linkid=2132578).</span><span class="sxs-lookup"><span data-stu-id="04a80-115">To learn how to access managed app logs, see [Use Microsoft Edge for iOS and Android to access managed app logs](https://go.microsoft.com/fwlink/?linkid=2132578).</span></span>
