---
title: مشكلة في AAD Connect Health
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480863"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="e0952-102">مشكلة في حالة اتصال AAD</span><span class="sxs-lookup"><span data-stu-id="e0952-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="e0952-103">تأكد من أنك مفوض لتنفيذ العملية.</span><span class="sxs-lookup"><span data-stu-id="e0952-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="e0952-104">يمكن للمسؤولين العامين الوصول بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="e0952-104">Global Admins have access by default.</span></span> <span data-ttu-id="e0952-105">بالإضافة إلى ذلك، يمكنك استخدام "التحكم بالوصول المستند [إلى الدور"](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) لتفويض إذن التسجيل للمساهم.</span><span class="sxs-lookup"><span data-stu-id="e0952-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="e0952-106">تأكد من تمكين نقاط النهاية المطلوبة، ومن عدم حظرها بسبب جدار الحماية.</span><span class="sxs-lookup"><span data-stu-id="e0952-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="e0952-107">للحصول على التفاصيل، راجع [المتطلبات.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)</span><span class="sxs-lookup"><span data-stu-id="e0952-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="e0952-108">قد يفشل التسجيل بسبب خضع الاتصال الصادر لفحص SSL بواسطة طبقة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="e0952-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="e0952-109">تأكد من أنك قمت بالتحقق من إعدادات الإعلامات الخاصة ب Azure AD Connect Health.</span><span class="sxs-lookup"><span data-stu-id="e0952-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="e0952-110">يرجى مراجعة الإعداد.</span><span class="sxs-lookup"><span data-stu-id="e0952-110">Please review your setting.</span></span> <span data-ttu-id="e0952-111">يمكن [أن](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) يساعدك هذا الدليل على فهم كيفية تكوين إعدادات الإعلامات لإعلامات Azure AD Connect الصحية.</span><span class="sxs-lookup"><span data-stu-id="e0952-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="e0952-112">لمعرفة المزيد حول تقرير مزامنة AAD Connect Health وكيفية تنزيله، راجع تقرير [مزامنة مستوى الكائن.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="e0952-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="e0952-113">استكشاف الأخطاء في تنبيهات AAD Connect Health وإصلاحها، اتبع دليل استكشاف الأخطاء وإصلاحها لتنبيهات سطوع بيانات [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) والأسئلة الشائعة، راجع أسئلة تثبيت [Common AAD Connect Health.](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)</span><span class="sxs-lookup"><span data-stu-id="e0952-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
