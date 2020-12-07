---
title: 'ادوار RBAC '
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003230"
- "7265"
ms.openlocfilehash: 7c4c9d1a76f395dfb2f831d555199b76c354ca57
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583172"
---
# <a name="rbac-rules"></a>قواعد RBAC

إذا حصلت علي خطا في الاذن: 

- لا **يتضمن العميل الذي يحتوي علي معرف العنصر تخويلا لتنفيذ الاجراء فوق النطاق (التعليمات البرمجية: أوثوريزاتيونفايليد)**: عند محاولة إنشاء مورد ، تاكد من انك قمت بتسجيل الدخول حاليا باستخدام مستخدم تم تعيين دور له اذن كتابه إلى المورد في النطاق المحدد. علي سبيل المثال ، لأداره الاجهزه الظاهرية في مجموعه موارد ، يجب ان يتوفر لديك دور [المساهم في الجهاز الظاهري](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#virtual-machine-contributor) علي مجموعه الموارد (أو النطاق الأصلي). للحصول علي قائمه بالأذونات لكل دور مضمن ، راجع [الأدوار المضمنة لموارد Azure](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support).
- **ليس لديك الاذن لإنشاء طلب دعم**: عند محاولة إنشاء بطاقة دعم أو تحديثها ، تاكد من انك قمت بتسجيل الدخول حاليا باستخدام المستخدم الذي تم تعيين دور له الذي يملك الاذن Microsoft. الدعم/سوبورتيكيتس/الكتابة ، مثل [الدعم المعتمد للطلب](https://docs.microsoft.com/azure/role-based-access-control/built-in-roles?WT.mc_id=Portal-Microsoft_Azure_Support#support-request-contributor).
- **لا يمكن إنشاء المزيد من تعيينات الأدوار (التعليمات البرمجية: روليسيجنمينتليميتيكسسيديد)**: عند محاولة تعيين دور ، حاول تقليل عدد تعيينات الدور عن طريق تعيين ادوار إلى المجموعات بدلا من ذلك. يدعم Azure تعيينات الأدوار حتى **2000** لكل اشتراك.

للحصول علي مزيد من التفاصيل حول ادوار Azure RBAC ، راجع [ادوار AZURE RBAC](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal?WT.mc_id=Portal-Microsoft_Azure_Support).
