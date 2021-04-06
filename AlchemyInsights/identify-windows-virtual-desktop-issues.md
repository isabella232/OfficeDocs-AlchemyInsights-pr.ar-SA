---
title: تحديد مشاكل سطح المكتب الظاهري ل Windows
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595424"
---
# <a name="identify-windows-virtual-desktop-issues"></a>تحديد مشاكل سطح المكتب الظاهري ل Windows

يستخدم Windows Virtual Desktop Diagnostics أمر cmdlet واحد فقط من PowerShell ولكنه يحتوي على العديد من المعلمات الاختيارية للمساعدة في تضييق المشاكل وعزلها. للبدء: 

1. قم بتنزيل الوحدة النمطية لسطح المكتب الظاهري ل Windows PowerShell واستيرادها. للحصول على التفاصيل، راجع [Windows Virtual Desktop Cmdlets ل Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).

1. قم بتشغيل cmdlet التالي تسجيل الدخول إلى حسابك:
    
    مثال: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`

**ملاحظة:** يجب أن تتضمن كل الاستعلامات التي تستخدم PowerShell المعلمتين -UserName أو -ActivityID. للحصول على قدرات المراقبة، راجع [استخدام Log Analytics لمميزة التشخيص](https://go.microsoft.com/fwlink/?linkid=2126847).

لتصفية الأنشطة التشخيصية حسب المستخدم، يمكنك تشغيل cmdlet التالي:

مثال: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`

توجد قائمة عوامل التصفية التي يمكنك تشغيلها لتشخيص المشاكل. لمعرفة المزيد حول تشخيص المشاكل، راجع التعرف على مشاكل سطح المكتب الظاهري ل [Windows وتشخصها](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).

لمعرفة المزيد حول الأخطاء الشائعة، راجع الأخطاء الشائعة [senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).
