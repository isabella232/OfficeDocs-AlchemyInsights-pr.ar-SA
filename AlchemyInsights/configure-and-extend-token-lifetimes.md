---
title: تكوين مدد الرمز المميز وتمديدها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/20/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7778"
- "9004351"
ms.openlocfilehash: 505e79ae9a163b89a6df2a7085480728bb0f1051
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/20/2021
ms.locfileid: "49916653"
---
# <a name="configure-and-extend-token-lifetimes"></a>تكوين مدد الرمز المميز وتمديدها

يمكنك تحديد مده بقاء access أو SAML أو الرمز المميز لمعرف تم إصداره بواسطة النظام الأساسي لهويه Microsoft. يمكنك تعيين اعمار الرموز المميزة لجميع التطبيقات في مؤسستك ، للحصول علي تطبيق متعدد المستاجرين (متعدد المؤسسات) ، أو لحساب خدمه معين في مؤسستك. للحصول علي مزيد من المعلومات ، أقرا [اعمار الرموز القابلة للتكوين](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).

للحصول علي أمثله ، أقرا [أمثله حول كيفيه تكوين مدد الرمز المميز](https://docs.microsoft.com/azure/active-directory/develop/configure-token-lifetimes).

لمعرفه كيفيه تكوين مده بقاء الرمز المميز وتوافقه في Azure Active directory B2C (Azure AD B2C) ، راجع [تكوين الرموز المميزة في Azure active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/configure-tokens?pivots=b2c-user-flow).

تصف المقالة [تكوين سلوك جلسة العمل في Azure Active DIRECTORY B2C](https://docs.microsoft.com/azure/active-directory-b2c/session-behavior?pivots=b2c-user-flow) طرق تسجيل الدخول الأحادي (SSO) المستخدمة في AZURE AD B2C وتساعدك علي اختيار أسلوب SSO الأكثر ملاءمة عند تكوين النهج.

**ما المدة التي تستغرقها الرموز المميزة في العمل ؟ ما المدة التي يكون فيها صالحا ؟**

اعمار الرموز المميزة هي 1 ساعة ومده بقاء جلسة العمل 24 ساعة. وهذا يعني انه إذا لم يتم اجراء اي طلبات في 24 ساعة ، ستحتاج إلى تسجيل الدخول مره أخرى قبل طلب رمز مميز جديد.

> [!NOTE]
> بعد 30 مايو 2020 ، لن يتمكن اي مستاجر جديد من استخدام نهج عمر الرمز المميز القابل للتكوين لتكوين جلسة العمل وتحديث الرموز المميزة. سيحدث إهمال خلال عده أشهر بعد ذلك ، مما يعني اننا سنقوم بإيقاف جلسة العمل الموجودة هونورينج وتحديث نهج الرموز المميزة. لا يزال بإمكانك تكوين مدد حياه الوصول بعد إهمال.






