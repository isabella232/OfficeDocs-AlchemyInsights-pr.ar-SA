---
title: مشكلات ترخيص Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148166"
---
# <a name="yammer-licensing-issues"></a>مشكلات ترخيص Yammer

يجب أن يكون لدى كافة المستخدمين ترخيص لاستخدام خدمة "المؤسسة Yammer" ولكن افتراضياً لا يتطلب Yammer أن يكون لدى المستخدمين ترخيص الوصول إلى الخدمة. عندما يقوم مسؤول بتغيير الإعداد لحظر مستخدمي Microsoft 365 بدون تراخيص Yammer، لا يمكن للمستخدمين الذين لم يتم تعيين ترخيص شركة Yammer الوصول إلى خدمة Yammer. لمزيد من المعلومات، راجع [إدارة تراخيص المستخدمين Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

عند إزالة التراخيص من المستخدمين، لم يعد يتم عرض الإطار المتجانب Yammer، كما يمكن استخدام خدمات أخرى إزالة الترخيص لإخفاء الميزات. وفي حالات أخرى، يمكن أن تظل الميزات تظهر ولكنها تتطلب تخصيص ترخيص للعمل.  

**الترخيص لا يتم تحديث للمستخدم**  

أحياناً، يتم تعيين ترخيص مستخدم ولكن لا يزال غير قادر على الوصول Yammer. من المحتمل حدوث التأخيرات عند وجود مهمة ترخيص كبيرة قيد التقدم. قد لا يتم تحديث المستخدمين Yammer بنفس الترتيب كما يتم تغيير التراخيص في إعلان Azure لأن النظام يعمل بشكل غير متزامن. انتظر حتى 24 ساعة قبل فتح حالة دعم للإبلاغ عن مشكلات مزامنة الترخيص.  

**تعيين الترخيص المجمع**  

يمكن تعيين التراخيص من خلال مركز الإدارة أو برمجة PowerShell النصية. لمزيد من المعلومات، راجع [تعيين التراخيص للمستخدمين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [وتعيين التراخيص لحسابات المستخدمين باستخدام Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

لا يوفر دعم Microsoft المساعدة في إنشاء البرامج النصية، ولكن تتوفر الوثائق الموجودة على تعيين ترخيص Yammer. لمزيد من المعلومات، راجع [إدارة تراخيص Yammer باستخدام Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).