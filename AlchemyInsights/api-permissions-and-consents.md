---
title: أذونات API وموافقتها
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932084"
---
# <a name="api-permissions-and-consent"></a>أذونات API وموافقتها

تتبع التطبيقات التي تتكامل مع النظام الأساسي للهويات في Microsoft نموذج تخويل يمنح المستخدمين والمسؤولين إمكانية التحكم في كيفية الوصول إلى البيانات. تم تحديث تنفيذ نموذج التفويض على النظام الأساسي للهويات في Microsoft النهاية. وهو يغير الطريقة التي يجب أن يتفاعل بها تطبيق مع النظام الأساسي للهويات في Microsoft. [تغطي الأذونات](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) النظام الأساسي للهويات في Microsoft نقطة النهاية المفاهيم الأساسية لنموذج التفويض هذا، بما في ذلك النطاقات والأذونات والموافقة.

يسهل [إطار عمل الموافقة ل Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) تطوير تطبيقات العميل الأصلية والويب متعددة المستأجرين. تسمح هذه التطبيقات بتسجيل الدخول بواسطة حسابات المستخدمين من مستأجر Azure AD الذي يختلف عن ذلك الذي تم تسجيل التطبيق فيه. وقد يحتاج أيضا إلى الوصول إلى واجهات برمجة تطبيقات الويب مثل واجهات برمجة تطبيقات Microsoft Graph (للوصول إلى Azure AD و Intune والخدمات في Microsoft 365) و واجهات برمجة تطبيقات خدمات Microsoft الأخرى، بالإضافة إلى واجهات برمجة تطبيقات الويب الخاصة بك.

