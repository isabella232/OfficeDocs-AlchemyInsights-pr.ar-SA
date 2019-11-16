---
title: ديناميات 365 نماذج قواعد العمل-قاعده الاعمال لا إطلاق النار لنموذج
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1926"
- "6200018"
ms.openlocfilehash: 3cdd2175083e864b3bffc57a70bb6c6220843fad
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "37769326"
---
# <a name="onchange-event-does-not-occur-if-the-field-is-changed-programmatically"></a><span data-ttu-id="5368e-102">لا يحدث الحدث OnChange إذا تم تغيير الحقل برمجيا</span><span class="sxs-lookup"><span data-stu-id="5368e-102">OnChange event does not occur if the field is changed programmatically</span></span>

<span data-ttu-id="5368e-103">لا يحدث الحدث *Onchange* إذا تم تغيير الحقل برمجيا باستخدام *السمة.* أسلوب [Setvalue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) .</span><span class="sxs-lookup"><span data-stu-id="5368e-103">The *OnChange* event does not occur if the field is changed programmatically using the *attribute.*[setValue](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/setvalue) method.</span></span> <span data-ttu-id="5368e-104">إذا كنت تريد معالجات الاحداث للحدث *Onchange* لتشغيل بعد تعيين القيمة يجب عليك استخدام *السمة formonchange. بيانات. الوحدة* [](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) في التعليمات البرمجية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="5368e-104">If you want event handlers for the *OnChange* event to run after you set the value you must use the *formContext.data.entity attribute* [fireOnchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/attributes/fireonchange) method in your code.</span></span>

[https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange](https://docs.microsoft.com/dynamics365/customer-engagement/developer/clientapi/reference/events/attribute-onchange)
