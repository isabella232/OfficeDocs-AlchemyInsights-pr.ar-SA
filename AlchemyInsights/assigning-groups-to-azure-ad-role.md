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
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2021
ms.locfileid: "49884761"
---
# <a name="assigning-groups-to-azure-ad-role"></a>تعيين مجموعات إلى دور Azure AD

لتعيين مجموعه Azure AD مع مصدر التخويل في Azure AD إلى دور Azure AD ، نفذ الخطوات التالية:

1. إنشاء مجموعه جديده-لإنشاء مجموعه جديده:

    علي. سجل دخولك إلى مركز أداره Azure AD باستخدام **مسؤول دور مميز** أو أذونات **المسؤول العام** .
    ب. حدد **مجموعات Azure Active directory > > كل المجموعات > المجموعة الجديدة**.
    ن. إنشاء المجموعة.

2. تعيين الدور إلى المجموعة اما اثناء إنشاء المجموعة أو بعد إنشاء المجموعة.

    علي. لتعيين دور إلى المجموعة في وقت إنشاء المجموعة ، يمكنك التبديل علي ادوار التبديل في **AZURE AD للمجموعة** وإنشاء المجموعة.
    ب. لتعيين دور إلى المجموعة بعد إنشائه ، انتقل إلى علامة التبويب **الأدوار المعينة** للمجموعة التي تم إنشاؤها حديثا ، وقم بتعيين الدور إلى المجموعة.  

**أداره عضويه مجموعه تم تعيينها إلى دور Azure AD**

لمنع رفع الامتيازات ، بشكل افتراضي ، يمكن لمسؤولي الأدوار المسموحين والمسؤولين العموميين فقط تعديل عضويه مجموعه تم تعيينها لأحد الأدوار. ومع ذلك ، يمكنك اختيار تعيين مالك لهذه المجموعة وتفويض هذه المهمة.

للحصول علي مزيد من التفاصيل حول تعيين مجموعات السحابة إلى ادوار Azure AD ، راجع [تعيين ادوار إعلانات إلى مجموعه السحابة](https://docs.microsoft.com/azure/active-directory/roles/groups-concept). للحصول علي مزيد من التفاصيل حول استكشاف الأخطاء وإصلاحها للأدوار المعينة إلى مجموعات السحابة ، راجع [استكشاف أخطاء الأدوار المعينة لمجموعات السحابة](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)





