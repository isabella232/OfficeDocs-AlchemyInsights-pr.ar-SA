---
title: إعلام AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034790"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="162de-102">إعلام AAD Connect</span><span class="sxs-lookup"><span data-stu-id="162de-102">Notification AAD Connect</span></span>

- <span data-ttu-id="162de-103">تأكد من أنك م مخولا لتنفيذ العملية.</span><span class="sxs-lookup"><span data-stu-id="162de-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="162de-104">يمكن للمسؤولين العامين الوصول بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="162de-104">Global Admins have access by default.</span></span> <span data-ttu-id="162de-105">بالإضافة إلى ذلك، يمكنك استخدام ["التحكم بالوصول المستند](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) إلى الدور" لتفويض إذن التسجيل إلى المساهم.</span><span class="sxs-lookup"><span data-stu-id="162de-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="162de-106">تأكد من تمكين نقاط النهاية المطلوبة، ولا يتم حظرها بسبب جدار الحماية.</span><span class="sxs-lookup"><span data-stu-id="162de-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="162de-107">للحصول على التفاصيل، راجع [المتطلبات](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="162de-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="162de-108">قد يفشل التسجيل بسبب تعرض الاتصال الصادر لفحص SSL بواسطة طبقة الشبكة.</span><span class="sxs-lookup"><span data-stu-id="162de-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="162de-109">تأكد من أنك قمت بالتحقق من إعدادات الإعلامات ل Azure AD Connect Health وراجع الإعداد.</span><span class="sxs-lookup"><span data-stu-id="162de-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="162de-110">لفهم كيفية تكوين إعدادات الإعلامات لإعلامات Azure AD Connect Health، راجع هذا [الدليل](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span><span class="sxs-lookup"><span data-stu-id="162de-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="162de-111">لمعرفة المزيد حول تقرير مزامنة AAD Connect Health وكيفية تنزيله، راجع تقرير مزامنة [مستوى الكائن](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span><span class="sxs-lookup"><span data-stu-id="162de-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="162de-112">لاستعلام تنبيهات حماية AAD Connect وإصلاحها، اتبع دليل استكشاف الأخطاء وإصلاحها لتنبيهات نضارة بيانات [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) والأسئلة الشائعة، راجع الأسئلة الشائعة حول تثبيت [AAD Connect Health](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="162de-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
