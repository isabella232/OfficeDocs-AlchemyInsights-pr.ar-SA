---
title: لا يظهر تطبيقي في "إدارة التطبيق"
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454398"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>لا يظهر تطبيقي في "إدارة التطبيق"

إذا لم يظهر التطبيق في إدارة التطبيق، فتحقق مما يلي:

1. انتقل إلى [Azure AD](https://aad.portal.azure.com/) وابحث عن "عرف التطبيق" لتطبيقك من خلال البحث عن اسم التطبيق في الشريط العلوي على صفحة نظرة عامة.

1. الوصول Graph مستكشف التطبيقات والبحث عن "المكتشف" داخل الخدمة الأساسية باستخدام هذا الاستعلام واستبداله بمكتشف التطبيق ذي <appId> الصلة: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> ">

1. إذا لم يتم إرجاع أي نتائج، فابحث عن "معرّف التطبيق" داخل التطبيق باستخدام هذا الاستعلام واستبداله بمرجع التطبيق ذي <appId> الصلة: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

إذا واجهت مشاكل في الاستعلام، فشاهد [الحصول على الدعم](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

لمزيد من المعلومات أو نظرة ثاقبة حول تطبيقاتك في إدارة التطبيق، راجع [التعرف على الرؤية والأفكار.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

لمزيد من المعلومات حول عرض تطبيقاتك، راجع [عرض تطبيقاتك](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
