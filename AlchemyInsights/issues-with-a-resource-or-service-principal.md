---
title: مشاكل تتعلق بالمورد أو الخدمة الأساسي
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
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/28/2021
ms.locfileid: "50713288"
---
# <a name="issues-with-a-resource-or-service-principal"></a>مشاكل تتعلق بالمورد أو الخدمة الأساسي

1. إذا كنت قد بدأت للتو، فإن كائنات التطبيق والخدمة الأساسية في [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) تصف تسجيل التطبيقات، وأشياء التطبيق، وأشياء الخدمة الأساسية في Azure Active Directory: ما هي هذه العناصر وكيفية استخدامها وكيفية اتسامها ببعضها البعض. يتم أيضا تقديم سيناريو مثال متعدد المستأجرين لتوضيح العلاقة بين كائن التطبيق للتطبيق والكائنات الأساسية المقابلة للخدمة.
2. يمكنك معرفة المزيد حول العلاقة بين التطبيقات وأهم الخدمات من خلال قراءة تطبيقات الخدمة والكائنات الأساسية [للخدمة في Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. كيفية: استخدام المدخل لإنشاء تطبيق [Azure AD](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) والخدمة الأساسية التي يمكنها الوصول إلى الموارد توضح لك كيفية إنشاء تطبيق Azure Active Directory (Azure AD) جديد وأهم خدمة يمكن استخدامها مع عنصر التحكم بالوصول المستند إلى الدور.
4. باستخدام [API الأساسي](https://docs.microsoft.com/graph/api/resources/serviceprincipal)للخدمة، يمكنك إدارة مثيلات التطبيقات برمجيا والتحكم في ما يمكن للتطبيق القيام به داخل نطاق المستأجر.
5. [يسرد نوع مورد servicePrincipal](https://docs.microsoft.com/graph/api/resources/serviceprincipal) جميع الخصائص والأساليب الخاصة بنوع مورد servicePrincipal.
6. تبرز الاختلافات بين نوع المورد [بين Azure AD Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) و Microsoft Graph الاختلافات بين Azure AD Graph وموارد Microsoft Graph. تعرض الموارد التي لها أسماء مختلفة أو غير متوفرة؛ ويسلط الضوء أيضا على الموارد المتوفرة في إصدار بيتا من Microsoft Graph ولكن ليس في الإصدار v1.0.

**مشاكل تتعلق بالمستخدمين الضيوف**

- [Quickstart:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Add guest users to your directory in the Azure portal shows you how to add a guest user to your Azure AD directory via the Azure portal, send an invitation, and see what the guest user's look like the invitation user's redemption process.
- البرنامج التعليمي: يمكنك إنشاء تدفقات المستخدم في [Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) لتظهر لك كيفية إنشاء بعض تدفقات المستخدمين المستحسنة باستخدام مدخل Azure. إذا كنت تبحث عن معلومات حول كيفية إعداد تدفق بيانات اعتماد كلمة مرور مالك المورد (ROPC) في التطبيق، فشاهد تكوين تدفق بيانات اعتماد كلمة مرور مالك المورد في Azure AD B2C.
