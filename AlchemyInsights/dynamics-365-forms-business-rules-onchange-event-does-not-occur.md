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
ms.openlocfilehash: cbdedd2c5fcf5517243e60e36d86479d6c3f7814
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529006"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a>لا يتم إجراء الحدث OnChange إذا تم تغيير الحقل برمجياً

لا يتم إجراء الحدث *OnChange* إذا تم تغيير الحقل برمجياً باستخدام *سمة.* أسلوب [setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) . إذا كنت تريد معالجات الأحداث لحدث *OnChange* لتشغيل بعد تعيين القيمة التي يجب أن تستخدمها *السمة formContext.data.entity.* [فيريونتشانجي](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) أسلوب في التعليمات البرمجية الخاصة بك.

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
