---
title: أذونات API والموافقة عليها
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
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974177"
---
# <a name="api-permissions-and-consent"></a>أذونات API والموافقة عليها

تتبع التطبيقات التي تتكامل مع النظام الأساسي لهويه Microsoft نموذج تخويل يمنح المستخدمين ويتحكم بالتحكم في كيفيه الوصول إلى البيانات. تم تحديث تطبيق نموذج التخويل علي نقطه نهاية النظام الأساسي لهويه Microsoft. انه يغير كيفيه تفاعل التطبيق مع النظام الأساسي للهوية من Microsoft. تغطي [الأذونات والموافقة في نقطه نهاية النظام الأساسي لهويه Microsoft](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) المفاهيم الاساسيه لنموذج التخويل هذا ، بما في ذلك النطاقات والأذونات والموافقة.

يسهل [اطار الموافقة علي Azure Active directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) تطوير تطبيقات العميل المتعددة علي ويب والمستاجرين. تسمح هذه التطبيقات بتسجيل الدخول بواسطة حسابات المستخدمين من مستاجر Azure AD والتي تختلف عن تلك التي تم تسجيل التطبيق فيها. قد يحتاج أيضا إلى الوصول إلى واجات برمجه التطبيقات علي الويب مثل Microsoft Graph API (للوصول إلى Azure AD و Intune والخدمات في Microsoft 365) وغيرها من واجات برمجه تطبيقات Microsoft services الأخرى ، بالاضافه إلى واجات برمجه تطبيقات ويب الخاصة بك.

