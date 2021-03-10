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
# <a name="troubleshoot-saml-signing-certificate-issues"></a>استكشاف مشاكل شهادة توقيع SAML وإصلاحها

لحل مشكلة شهادة توقيع SAML، تنفيذ الخطوات الموصى بها التالية:

1. عند إضافة تطبيق مؤسسة يدعم SSO، ينشئ Azure شهادة تسمى شهادة توقيع [SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) تاريخ انتهاء صلاحية هذه الشهادة هو 3 سنوات. لتغيير تاريخ انتهاء صلاحية الشهادة، راجع تخصيص تاريخ انتهاء صلاحية شهادة الاتحاد الخاصة بك ثم تسليمها [إلى شهادة جديدة.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)
2. سيستخدم Azure هذه الشهادة لتوقيع رموز SAML المميزة التي يطلبها التطبيق ويرسلها إلى التطبيق للحصول على تسجيل الدخول SSO بنجاح. لكي يتم ذلك، قم بتنزيل الشهادة من مدخل Azure وأرسلها إلى مورد التطبيق لإكمال عملية SSO.

بعد اكتمال هذه العملية، سيثق التطبيق بهذه الشهادة وسيقبل التطبيق جميع رموز SAML المميزة الموقعة بواسطة هذه الشهادة.

3. إذا تنتهي صلاحية هذه الشهادة، فنشئ شهادة جديدة، ثم قم بتحديثها إلى مورد التطبيق ثم اجعلها نشطة على جانب Azure. لمزيد من المعلومات، راجع ["تجديد شهادة" ستنتهي صلاحيتها قريبا.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)

> [!NOTE]
> إذا تنتهي صلاحية الشهادة، لن يتم حظر المستخدم.

4. [أضف عنوان بريد إلكتروني لكي يتم تلقي](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) الإعلامات قبل انتهاء صلاحية الشهادة الحالية.

> [!NOTE]
> الخطوة 4 هي خطوة اختيارية.

5. تغيير خيارات توقيع شهادة SAML الخاصة بتطبيق وخوارزمية توقيع الشهادة. لمزيد من المعلومات، راجع [تغيير خيارات توقيع الشهادة وخوارزمية التوقيع.](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)

