---
title: إعداد شهادة APNS لإدارة Intune لأجهزة iOS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "3543"
ms.openlocfilehash: 027e1e0fa3b625fa0f619bc6d74844f6ec5be769
ms.sourcegitcommit: 75346a972c2174248de3bb55a19d714cee43c1cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/09/2020
ms.locfileid: "43211161"
---
# <a name="intune-ios-set-up-apns-certificate"></a><span data-ttu-id="a2165-102">إعداد شهادة APNS لإدارة Intune لأجهزة iOS</span><span class="sxs-lookup"><span data-stu-id="a2165-102">Intune iOS set up APNS certificate</span></span>

<span data-ttu-id="a2165-103">لم يتم تكوين الشهادة المؤقتة لإدارة الأجهزة المحمولة من Apple (المعروفة أيضاً باسم شهادة خدمة الإعلامات المؤقتة من Apple (APNS)) على اشتراكك.</span><span class="sxs-lookup"><span data-stu-id="a2165-103">An Apple MDM Push certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured on your subscription.</span></span>

<span data-ttu-id="a2165-104">بدون توفر شهادة مؤقتة لإدارة الأجهزة المحمولة من Apple تم تكوينها، لن تتمكن من تسجيل أجهزة iOS وMacOS وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="a2165-104">Without an Apple MDM Push certificate configured, you'll be unable to enroll and manage iOS and MacOS devices.</span></span> <span data-ttu-id="a2165-105">بعد أن تضيف الشهادة إلى Intune، سيتمكن المستخدمين لديك من تثبيت تطبيق Company Portal لتسجيل أجهزة iOS الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="a2165-105">After you add the certificate to Intune, your users can install the Company Portal app to enroll their iOS devices.</span></span>

<span data-ttu-id="a2165-106">للحصول على إرشادات خطوة بخطوة حول إضافة شهادة APNS إلى مستأجر Intune لديك، الرجاء مراجعة المحتوى الوارد في الارتباط التالي:</span><span class="sxs-lookup"><span data-stu-id="a2165-106">For a step-by-step guide to adding an APNS certificate to your Intune tenant, please review the content on the following link:</span></span>

- [<span data-ttu-id="a2165-107">الحصول على الشهادة المؤقتة لإدارة الأجهزة المحمولة من Apple</span><span class="sxs-lookup"><span data-stu-id="a2165-107">Get an Apple MDM Push certificate</span></span>](https://docs.microsoft.com/mem/intune/enrollment/apple-mdm-push-certificate-get)

<span data-ttu-id="a2165-108">إذا كنت تواجه مشاكل في شهادة الإعلام المؤقتة من Apple (APNs)، فراجع منشور المدوّنة التالي: [Intune وشهادة APNs: الأسئلة المتداولة والمشاكل الشائعة](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span><span class="sxs-lookup"><span data-stu-id="a2165-108">If you are having issues with the Apple Push Notification certificate (APNs) refer to this blog post: [Intune and the APNs certificate: FAQ and common issues](https://techcommunity.microsoft.com/t5/Intune-Customer-Success/Intune-and-the-APNs-certificate-FAQ-and-common-issues/ba-p/280121)</span></span>
