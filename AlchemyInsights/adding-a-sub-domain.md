---
title: إضافة مجال فرعي
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506183"
---
# <a name="adding-a-sub-domain"></a>إضافة مجال فرعي

يمكن إضافة المجالات الفرعية إلى المستأجر نفسه أو إلى نطاق مستأجر مختلف عن المجال الأصل. وفي كلتا الحالتين، يجب إدارة إعدادات DNS الخاصة بك في موقع جهة التسجيل على الويب. إذا سمحت ل Microsoft بإدارة إعدادات DNS باستخدام سجلات NS، أو إذا اشتريت المجال من Microsoft، فلن تتمكن من إضافة المجالات الفرعية دون تغيير هذا أولا.

أضف المجال الأصل أولا ثم أضف المجال الفرعي. إذا كان مجال العمل الفرعي في المستأجر نفسه، فلا حاجة إلى التحقق من صحة إضافية. إذا قمت بإضافة المجال الفرعي إلى مستأجر منفصل، يكون سجل DNS txt مطلوبا للتحقق من الملكية قبل إضافة المجال وسجلات DNS الإضافية للخدمات المحددة.

- لإضافة مجال أو مجال فرعي، اتبع المعالج إضافة مجال [،](https://admin.microsoft.com/Adminportal#/Domains/Wizard)أو أضف المجال أو المجال الفرعي يدويا عن طريق الذهاب إلى **إعداد**  >  **المجالات**  >  **إضافة مجال**.

إذا لزم الأمر:

- لتغيير الأشخاص الذين يديرون إعدادات DNS لمجال موجود، انتقل إلى **الإعدادات** المجالات ، وحدد خانة الاختيار الموجودة بجانب المجال، ثم  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)حدد **إدارة DNS**. في المعالج، حدد **إضافة سجلات DNS** الخاصة بك وإكمال المعالج.
- لإضافة مجالات فرعية إلى مجال تم شراؤه من Microsoft، قم أولا بنقل المجال إلى جهة تسجيل أخرى، ثم قم بالتغيير أعلاه لإدارة سجلات DNS الخاصة بك. للحصول على الإرشادات، راجع [نقل مجال من Microsoft إلى مضيف آخر](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host).
- إذا تلقيت رسالة خطأ بأن مجالك مستخدم بالفعل من قبل أعضاء آخرين أو أشخاص آخرين في مؤسستك، ستحتاج أولا إلى التولى هذا الحساب غير مدار قبل استخدام المجال. للحصول على الإرشادات، راجع إدارة دليل غير مدار [كمسؤول في Azure Active Directory](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover).
