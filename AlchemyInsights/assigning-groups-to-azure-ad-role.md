---
title: تعيين مجموعات إلى دور Azure AD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: 563b1a7c93c9ca64fdea51c57b70fd2132750c4ad8ee15de0c65c9668c9c3c56
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54036227"
---
# <a name="assigning-groups-to-azure-ad-role"></a>تعيين مجموعات إلى دور Azure AD

لتعيين مجموعة Azure AD ذات مصدر مرجع في Azure AD إلى دور Azure AD، قم بتنفيذ الخطوات التالية:

1. إنشاء مجموعة جديدة - لإنشاء مجموعة جديدة:

    a. سجل الدخول إلى مركز إدارة Azure AD باستخدام **أذونات مسؤول** الدور المميز أو **المسؤول** العام.
    b. حدد **Azure Active Directory > مجموعات > كافة المجموعات > مجموعة جديدة**.
    c. إنشاء المجموعة.

2. قم بتعيين الدور إلى المجموعة إما أثناء إنشاء المجموعة أو بعد إنشائها.

    a. لتعيين دور إلى المجموعة في وقت إنشاء المجموعة، قم بالتبديل بين أدوار **Azure AD** التي يمكن تعيينها إلى المجموعة وإنشاء المجموعة.
    b. لتعيين دور إلى المجموعة بعد إنشائها، انتقل إلى  علامة التبويب الأدوار المعينة للمجموعة التي تم إنشاؤها حديثا، ثم قم بتعيين الدور إلى المجموعة.  

**إدارة عضوية مجموعة معينة إلى دور Azure AD**

لمنع رفع الامتيازات، بشكل افتراضي، يمكن لمسؤولي الدور المميزين والمسؤولين العامين فقط تعديل عضوية مجموعة معينة إلى دور. ومع ذلك، يمكنهم اختيار تعيين مالك لهذه المجموعة وتفويض هذه المهمة.

للحصول على مزيد من التفاصيل حول تعيين مجموعات سحابية إلى أدوار Azure AD، راجع [تعيين أدوار AD إلى مجموعة السحابة](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). للحصول على مزيد من التفاصيل حول استكشاف الأخطاء وإصلاحها التي تم تعيينها لمجموعات السحابة، راجع استكشاف الأخطاء وإصلاحها التي تم تعيينها [للمجموعات السحابية](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).





