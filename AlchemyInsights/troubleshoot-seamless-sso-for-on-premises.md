---
title: استكشاف الأخطاء في تسجيل الدخول الفردي السلس (SSO) وإصلاحها في الموقع المحلي
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816059"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="20e6c-102">استكشاف الأخطاء في تسجيل الدخول الفردي السلس (SSO) وإصلاحها في الموقع المحلي</span><span class="sxs-lookup"><span data-stu-id="20e6c-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="20e6c-103">لحل مشاكل تسجيل الدخول الفردي السلس ( SSO)، قم بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="20e6c-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="20e6c-104">**كيف يمكنني تجاوز مفتاح فك تشفير Kerberos لحساب الكمبيوتر AZUREADSSO؟**</span><span class="sxs-lookup"><span data-stu-id="20e6c-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="20e6c-105">نوصي بشدة بقلب مفتاح فك تشفير Kerberos كل 30 يوما على الأقل.</span><span class="sxs-lookup"><span data-stu-id="20e6c-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="20e6c-106">للقيام بذلك يدويا، راجع كيفية طرح مفاتيح فك تشفير [Kerberos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span><span class="sxs-lookup"><span data-stu-id="20e6c-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="20e6c-107">**تكوين SSO السلس**</span><span class="sxs-lookup"><span data-stu-id="20e6c-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="20e6c-108">لنشر تسجيل الدخول الموحد السلس، اتبع الخطوات في تسجيل الدخول المفرد السلس في [Azure Active Directory: التشغيل السريع](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span><span class="sxs-lookup"><span data-stu-id="20e6c-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="20e6c-109">**استشارات**</span><span class="sxs-lookup"><span data-stu-id="20e6c-109">**Advisory**</span></span>

- <span data-ttu-id="20e6c-110">تسجيل الدخول الفردي السلس في [Azure Active Directory:](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) الأسئلة التي يتم طرحها بشكل متكرر - في هذه المقالة، نعالج الأسئلة التي يتم طرحها بشكل متكرر حول Azure Active Directory تسجيل الدخول الفردي السلس Sign-On (تسجيل الدخول السلس).</span><span class="sxs-lookup"><span data-stu-id="20e6c-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="20e6c-111">استمر في التحقق مرة أخرى من المحتوى الجديد.</span><span class="sxs-lookup"><span data-stu-id="20e6c-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="20e6c-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - توفر هذه المقالة معلومات حول كيفية تقديم طلبات الميزات أو طرح أسئلة تقنية حول SSO السلس.</span><span class="sxs-lookup"><span data-stu-id="20e6c-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="20e6c-113">**استكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="20e6c-113">**Troubleshoot**</span></span>

<span data-ttu-id="20e6c-114">استكشاف الأخطاء وإصلاحها تسجيل الدخول الفردي السلس إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - تساعدك هذه المقالة على العثور على معلومات حول استكشاف الأخطاء وإصلاحها حول المشاكل الشائعة المتعلقة ب Azure Active Directory (Azure AD) تسجيل الدخول المفرد السلس Sign-On (تسجيل الدخول الموحد السلس).</span><span class="sxs-lookup"><span data-stu-id="20e6c-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







