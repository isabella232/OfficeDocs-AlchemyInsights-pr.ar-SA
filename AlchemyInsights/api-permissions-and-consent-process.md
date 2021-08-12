---
title: أذونات API وعملية الموافقة
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
- "9004345"
- "9200"
ms.openlocfilehash: 078f5798533dfbbf97858f305729f103663644fee3590cdcc877233041adae81
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932048"
---
# <a name="api-permissions-and-consent-process"></a>أذونات API وعملية الموافقة

لكي يمكن لتطبيقك الوصول إلى البيانات في Microsoft Graph، يجب على المستخدم أو المسؤول منحه الأذونات الصحيحة عبر عملية موافقة. [يسرد Graph](https://docs.microsoft.com/graph/permissions-reference) أذونات Microsoft الأذونات المقترنة بكل مجموعة رئيسية من واجهات برمجة التطبيقات Graph Microsoft. كما يوفر إرشادات حول كيفية استخدام الأذونات.

**إعداد الخدمة الأساسية أو تحديثها**

- [إنشاء serviceprincipal](https://docs.microsoft.com/graph/api/serviceprincipal-post-serviceprincipals) - توضح لك هذه المقالة كيفية إنشاء كائن servicePrincipal جديد.
- إنشاء [تطبيق Azure AD &](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) أساسي للخدمة في المدخل - توضح لك هذه المقالة كيفية إنشاء تطبيق Azure Active Directory (Azure AD) جديد وأهم خدمة يمكن استخدامها مع عنصر تحكم الوصول المستند إلى الدور.
- تطبيقات & أساسيات الخدمات في [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) - تصف هذه المقالة تسجيل التطبيقات، وأشياء التطبيقات، وأعراض الخدمة الأساسية في Azure Active Directory: ماهيتها وكيفية استخدامها وكيفية اتسامها ببعضها البعض.

**إضافة تسجيل التطبيق أو تحديثه وتقديم موافقة المسؤول**

- [إنشاء تسجيل تطبيق](https://docs.microsoft.com/graph/api/application-post-applications) - توضح لك هذه المقالة كيفية إنشاء كائن تطبيق جديد.
- [تحديث تسجيل تطبيق - أذونات API](https://docs.microsoft.com/graph/api/application-update) - توضح لك هذه المقالة كيفية تحديث خصائص كائن تطبيق.
- [تقديم موافقة المسؤول](https://docs.microsoft.com/graph/security-authorization#grant-permissions-to-an-application) - لموافقة المسؤول وموافقته بشكل عام، نطلب من المسؤول منح الموافقة بشكل صريح.
- [RBAC (beta)](https://docs.microsoft.com/graph/api/resources/rbacapplicationmultiple) - حاوية إدارة الدور لتعريفات الدور الموحدة وواجبات الدور لموفري Microsoft 365 RBAC الذين يدعمون العديد من الأساسيات والنطاقات المتعددة في تعيين دور واحد. يختلف ذلك عن نوع مورد *rbacApplication.* Microsoft Intune مثال لموفر RBAC هذا. يمكن أن يكون تعيين الدور في Intune صفيفا من الأساسيات صفيفا من مجموعات النطاقات. **هذا الإصدار في الإصدار بيتا، مما يعني أنه لا يزال قيد التطوير ولا يوصى باستخدامه في الإنتاج.**
