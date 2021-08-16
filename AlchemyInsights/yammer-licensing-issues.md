---
title: Yammer مشاكل الترخيص
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 3ec764ece9cb7be933e9e2cd002379898522790528b0fa586ab501424b00cd7b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53989716"
---
# <a name="yammer-licensing-issues"></a>Yammer مشاكل الترخيص

يجب أن يكون لدى جميع المستخدمين ترخيصا لاستخدام Yammer Enterprise، ولكن لا يتطلب Yammer المستخدمين الحصول على ترخيص للوصول إلى الخدمة. عندما يقوم أحد المسؤولين بتغيير الإعداد لحظر Microsoft 365 الذين لا Yammer تراخيص، لا يمكن للمستخدمين الذين لم يتم تعيين Yammer Enterprise الوصول إلى Yammer الخدمة. لمزيد من المعلومات، [راجع إدارة Yammer المستخدمين في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

عند إزالة التراخيص من المستخدمين، لن Yammer عرض لوحة التراخيص، ويمكن للخدمات الأخرى استخدام إزالة الترخيص لإخفاء الميزات. وفي حالات أخرى، لا يزال من الممكن أن تظهر الميزات ولكنها تتطلب تعيين ترخيص للعمل.  

**لا يتم تحديث الترخيص للمستخدم**  

في بعض الأحيان، يتم تعيين ترخيص للمستخدم ولكنه لا يزال غير قادر على الوصول إلى Yammer. من المرجح أن تحدث التأخيرات عندما يكون تعيين التراخيص الجماعية في تقدم. Yammer عدم تحديث المستخدمين بنفس ترتيب تغيير التراخيص في Azure AD بسبب تشغيل النظام بشكل غير متزامن. انتظر حتى 24 ساعة قبل فتح حالة دعم للتقارير حول مشاكل مزامنة الترخيص.  

**تعيين ترخيص مجمع**  

يمكن تعيين التراخيص من خلال مركز الإدارة أو البرمجة النصية في PowerShell. لمزيد من المعلومات، راجع [تعيين تراخيص](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) للمستخدمين وتعيين تراخيص إلى حسابات المستخدمين باستخدام Office 365 [PowerShell.](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell) 

لا يوفر دعم Microsoft المساعدة في إنشاء البرامج النصية، ولكن الوثائق Yammer تعيين الترخيص متوفرة. لمزيد من المعلومات، [راجع إدارة Yammer باستخدام Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).