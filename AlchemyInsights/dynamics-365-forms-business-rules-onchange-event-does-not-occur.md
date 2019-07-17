---
title: قواعد العمل-لا يطلقون النار لنموذج قاعدة العمل يشكل Dynamics 365
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 4ade8d2f68b465298e2d6efff3eef4f04f25c3bf
ms.sourcegitcommit: a413a0e27ef4ab8c484fa9fccff8bbef381c8b96
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2019
ms.locfileid: "35746803"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>لا يتم إجراء الحدث OnChange إذا تم تغيير الحقل برمجياً

لا يتم إجراء الحدث *OnChange* إذا تم تغيير الحقل برمجياً باستخدام *سمة.* أسلوب [setValue](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . إذا كنت تريد معالجات الأحداث لحدث *OnChange* لتشغيل بعد تعيين القيمة التي يجب أن تستخدمها *السمة formContext.data.entity.* [فيريونتشانجي](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) أسلوب في التعليمات البرمجية الخاصة بك.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/en-us/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
