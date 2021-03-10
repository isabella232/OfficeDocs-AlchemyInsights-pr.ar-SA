---
title: استكشاف مشاكل شهادة توقيع SAML وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50692398"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="580f5-102">استكشاف مشاكل شهادة توقيع SAML وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="580f5-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="580f5-103">لحل مشكلة شهادة توقيع SAML، تنفيذ الخطوات الموصى بها التالية:</span><span class="sxs-lookup"><span data-stu-id="580f5-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="580f5-104">عند إضافة تطبيق مؤسسة يدعم SSO، ينشئ Azure شهادة تسمى شهادة توقيع [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications)</span><span class="sxs-lookup"><span data-stu-id="580f5-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="580f5-105">تاريخ انتهاء صلاحية هذه الشهادة هو 3 سنوات.</span><span class="sxs-lookup"><span data-stu-id="580f5-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="580f5-106">لتغيير تاريخ انتهاء صلاحية الشهادة، راجع تخصيص تاريخ انتهاء صلاحية شهادة الاتحاد الخاصة بك ثم تسليمها [إلى شهادة جديدة.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)</span><span class="sxs-lookup"><span data-stu-id="580f5-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="580f5-107">سيستخدم Azure هذه الشهادة لتوقيع رموز SAML المميزة التي يطلبها التطبيق ويرسلها إلى التطبيق للحصول على تسجيل الدخول SSO بنجاح.</span><span class="sxs-lookup"><span data-stu-id="580f5-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="580f5-108">لكي يتم ذلك، قم بتنزيل الشهادة من مدخل Azure وأرسلها إلى مورد التطبيق لإكمال عملية SSO.</span><span class="sxs-lookup"><span data-stu-id="580f5-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="580f5-109">بعد اكتمال هذه العملية، سيثق التطبيق بهذه الشهادة وسيقبل التطبيق جميع رموز SAML المميزة الموقعة بواسطة هذه الشهادة.</span><span class="sxs-lookup"><span data-stu-id="580f5-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="580f5-110">إذا تنتهي صلاحية هذه الشهادة، فنشئ شهادة جديدة، ثم قم بتحديثها إلى مورد التطبيق ثم اجعلها نشطة على جانب Azure.</span><span class="sxs-lookup"><span data-stu-id="580f5-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="580f5-111">لمزيد من المعلومات، راجع ["تجديد شهادة" ستنتهي صلاحيتها قريبا.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)</span><span class="sxs-lookup"><span data-stu-id="580f5-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="580f5-112">إذا تنتهي صلاحية الشهادة، لن يتم حظر المستخدم.</span><span class="sxs-lookup"><span data-stu-id="580f5-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="580f5-113">[أضف عنوان بريد إلكتروني لكي يتم تلقي](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) الإعلامات قبل انتهاء صلاحية الشهادة الحالية.</span><span class="sxs-lookup"><span data-stu-id="580f5-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="580f5-114">الخطوة 4 هي خطوة اختيارية.</span><span class="sxs-lookup"><span data-stu-id="580f5-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="580f5-115">تغيير خيارات توقيع شهادة SAML الخاصة بتطبيق وخوارزمية توقيع الشهادة.</span><span class="sxs-lookup"><span data-stu-id="580f5-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="580f5-116">لمزيد من المعلومات، راجع [تغيير خيارات توقيع الشهادة وخوارزمية التوقيع.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)</span><span class="sxs-lookup"><span data-stu-id="580f5-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

