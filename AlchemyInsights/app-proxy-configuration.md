---
title: تكوين وكيل التطبيق
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
- "9004356"
- "7800"
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884771"
---
# <a name="app-proxy-configuration"></a><span data-ttu-id="d7dcc-102">تكوين وكيل التطبيق</span><span class="sxs-lookup"><span data-stu-id="d7dcc-102">App Proxy Configuration</span></span>

1. <span data-ttu-id="d7dcc-103">لفهم كيفيه تكوين تطبيق وكيل التطبيق داخل Azure AD لعرض تطبيقاتك المحلية إلى السحابة ، راجع [كيفيه تكوين تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span><span class="sxs-lookup"><span data-stu-id="d7dcc-103">To understand how to configure an Application Proxy application within Azure AD to expose your on-premises applications to the cloud, see [How to configure an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).</span></span>
2. <span data-ttu-id="d7dcc-104">يسمح تسجيل الدخول الأحادي (SSO) للمستخدمين بالوصول إلى أحد التطبيقات من دون المصادقة عده مرات.</span><span class="sxs-lookup"><span data-stu-id="d7dcc-104">Single sign-on (SSO) allows your users to access an application without authenticating multiple times.</span></span> <span data-ttu-id="d7dcc-105">يسمح هذا الأمر للمصادقة بان تحدث في السحابة ، مقابل Azure Active Directory ، وتسمح للخدمة أو الموصل بانتحال المستخدم لإكمال اي تحديات مصادقه اضافيه من التطبيق.</span><span class="sxs-lookup"><span data-stu-id="d7dcc-105">It allows the single authentication to occur in the cloud, against Azure Active Directory, and allows the service or Connector to impersonate the user to complete any additional authentication challenges from the application.</span></span> <span data-ttu-id="d7dcc-106">لمعرفه المزيد ، راجع [كيفيه تكوين تسجيل الدخول الأحادي إلى تطبيق وكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span><span class="sxs-lookup"><span data-stu-id="d7dcc-106">To learn more, see [How to configure single sign-on to an Application Proxy application](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).</span></span>
3. <span data-ttu-id="d7dcc-107">استخدم [هذه المقالة](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) لاستكشاف المشاكل الشائعة التي تواجه الأشخاص وإصلاحها عند إنشاء تطبيق جديد لوكيل التطبيق.</span><span class="sxs-lookup"><span data-stu-id="d7dcc-107">Use [this article](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) to troubleshoot common issues people face when creating a new application proxy application.</span></span>
4. <span data-ttu-id="d7dcc-108">إذا كنت تواجه مشكله في اعداد المصادقة النهائية للتطبيق ، فقد تحتاج إلى [استكشاف الأخطاء في تكوينات التفويض المقيدة ل Kerberos لوكيل التطبيق](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) أو اتباع الإرشادات المتعلقة [بتكوين التطبيق باستخدام بينجاكسيس](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) لحل مشكلتك.</span><span class="sxs-lookup"><span data-stu-id="d7dcc-108">If you are having a problem setting up back-end authentication to your application you may need to [Troubleshoot Kerberos constrained delegation configurations for Application Proxy](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) or follow guidance on [configuring application with PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) to resolve your issue.</span></span>
