---
title: حذف المستاجر
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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564355"
---
# <a name="delete-tenant"></a>حذف المستاجر

لحذف Azure AD ، تاكد من:
- أنت مسؤول عام علي الدليل.
- لم يتم تسجيل دخولك باستخدام حساب لديه الدليل الافتراضي مثل contoso.onmicrosoft.com في الحساب الذي تم تسجيل دخوله ، مثل admin@contoso.onmicrosoft.com.
- قم بازاله اي تطبيقات نشطه في الدليل قبل الحذف. لأزاله التطبيقات النشطة ، انتقل إلى تسجيلات التطبيق وأزاله التطبيقات الموجودة.
- لا توجد اي اشتراكات نشطه لأي من خدمات Microsoft عبر الإنترنت ، مثل Microsoft Azure أو Office 365 أو Azure AD Premium المقترنة بالدليل. يمكنك نقل الاشتراكات أو تسريع إلغاء الاشتراكات النشطة عبر دعم Azure والفوترة. تعرف علي المزيد حول كيفيه إلغاء اشتراكات Office 365 و Azure. للحصول علي إرشادات حول اقران اشتراك موجود أو اضافته إلى المستاجر ، راجع [اقران اشتراك azure أو اضافته إلى مستاجر AZURE AD](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- لا يوجد ترخيص نشط. لأزاله التراخيص ، راجع [كيفيه أزاله الاشتراك لأزاله الترخيص](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- لا يوجد اي مستخدمين نشطين آخرين في الدليل بجانب نفسك كالمسؤول العام عند محاولة حذف Azure AD. قم بازاله اي مستخدمين آخرين نشطين ، سيحتاج اي تبعيات علي اسم مجال مخصص في المستاجر إلى ازالته ، مثل المستخدمين الذين تم إنشاؤهم باستخدام admin@contoso.com.

لمزيد من الخطوات التفصيلية حول كيفيه القيام بما يلي:
- حذف "Azure Active directory" أو "الاشتراك" ، راجع [حذف Azure active](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)directory.
- أزاله التطبيقات في الدليل ، راجع [أزاله التطبيقات](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
