---
title: حذف المستأجر
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993880"
---
# <a name="delete-tenant"></a>حذف المستأجر

لحذف Azure AD، تأكد من:
- أنت مسؤول عام في الدليل.
- لم يتم توقيعك باستخدام حساب به الدليل الافتراضي مثل contoso.onmicrosoft.com في الحساب الذي تم توقيعه، مثل admin@contoso.onmicrosoft.com.
- قم بإزالة أي تطبيقات نشطة في الدليل قبل الحذف. لإزالة التطبيقات النشطة، انتقل إلى تسجيلات التطبيقات وأزل التطبيقات الموجودة.
- لا توجد اشتراكات نشطة لأي من خدمات Microsoft Online، مثل Microsoft Azure أو Office 365 أو Azure AD Premium المقترنة في الدليل. نقل اشتراكاتك أو تسريع إلغاء الاشتراكات النشطة عبر دعم Azure و الفوترة. تعرف على المزيد حول كيفية إلغاء اشتراكات Office 365 و Azure. للحصول على إرشادات حول إقران اشتراك موجود أو إضافته إلى مستأجر، راجع إقران اشتراك Azure أو إضافته إلى [مستأجر Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- لا يوجد ترخيص نشط. لإزالة التراخيص، [راجع كيفية إزالة الاشتراك لإزالة الترخيص](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- لا يوجد مستخدمون نشطون آخرون في الدليل إلى جانب نفسك كمسؤول عام عند محاولة حذف Azure AD. قم بإزالة أي مستخدمين نشطين آخرين، وستحتاج أيضا أي تبعيات على اسم مجال مخصص في نطاق المستأجر إلى إزالتها، مثل المستخدمين الذين تم إنشاؤهم باستخدام admin@contoso.com.

للحصول على مزيد من الخطوات حول كيفية:
- حذف "Azure Active Directory" أو "اشتراك"، راجع [حذف Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- إزالة التطبيقات في الدليل، راجع [إزالة التطبيقات](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
