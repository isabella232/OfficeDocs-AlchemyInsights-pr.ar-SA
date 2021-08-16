---
title: المشاكل المتعلقة بالمورد أو الخدمة الأساسية
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
- "9004336"
- "7741"
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028063"
---
# <a name="issues-with-a-resource-or-service-principal"></a>المشاكل المتعلقة بالمورد أو الخدمة الأساسية

1. إذا كنت قد بدأت للتو، فإن العناصر الأساسية للتطبيقات والخدمات في [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) تصف تسجيل التطبيقات، وأشياء التطبيق، وأشياء الخدمة الأساسية في Azure Active Directory: ماهيتها، وكيفية استخدامها، وكيفية اتسامها ببعضها البعض. يتم أيضا تقديم سيناريو مثال متعدد المستأجرين لتوضيح العلاقة بين كائن تطبيق التطبيق والكائنات الأساسية المقابلة للخدمة.
2. يمكنك معرفة المزيد حول العلاقة بين التطبيقات ومديري الخدمات من خلال قراءة التطبيقات والأشياء [الأساسية للخدمة في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. كيفية: استخدم المدخل لإنشاء تطبيق [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) وأهم خدمة يمكنها الوصول إلى الموارد توضح لك كيفية إنشاء تطبيق Azure Active Directory (Azure AD) جديد وأهم خدمة يمكن استخدامها مع عنصر تحكم الوصول المستند إلى الدور.
4. باستخدام [API الأساسية للخدمة](https://docs.microsoft.com/graph/api/resources/serviceprincipal)، يمكنك إدارة مثيلات التطبيقات برمجيا والتحكم في ما يمكن للتطبيق القيام به داخل المستأجر.
5. [نوع مورد servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) يسرد كل الخصائص والأساليب لنوع مورد servicePrincipal.
6. تسلط الاختلافات بين نوع المورد [Graph Azure AD](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) و Microsoft Graph الضوء على الاختلافات بين Azure AD Graph و Microsoft Graph الموارد. وهي تعرض الموارد التي لها أسماء مختلفة أو غير متوفرة؛ كما يسلط الضوء على الموارد المتوفرة في إصدار بيتا من Microsoft Graph ولكن ليس في الإصدار 1.0.

**المشاكل المتعلقة بالمستخدمين الضيوف**

- [Quickstart:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) إضافة مستخدمين ضيوف إلى الدليل في مدخل Azure يوضح لك كيفية إضافة مستخدم ضيف جديد إلى دليل Azure AD عبر مدخل Azure، وإرسال دعوة، وترى كيف تبدو عملية استرداد دعوة المستخدم الضيف.
- البرنامج التعليمي: يعرض لك إنشاء تدفقات المستخدمين في [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) كيفية إنشاء بعض تدفقات المستخدمين المستحسنة باستخدام مدخل Azure. إذا كنت تبحث عن معلومات حول كيفية إعداد تدفق بيانات اعتماد كلمة مرور مالك المورد (ROPC) في التطبيق، فاطلع على تكوين تدفق بيانات اعتماد كلمة مرور مالك المورد في Azure AD B2C.
