---
title: نشر الوظائف الإضافية Microsoft 365 Apps
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/30/2021
ms.locfileid: "52124784"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>نشر الوظائف الإضافية Microsoft 365 Apps

النشر المركزي هو الطريقة المستحسنة لنشر Office الإضافية للمستخدمين والمجموعات داخل مؤسستك. لنشر الوظائف الإضافية، اتبع الخطوات أدناه:

**ملاحظة:** لتثبيت الوظائف الإضافية Office كمستخدم فردي، راجع عرض الوظائف الإضافية وإدارتها وتثبيتها في برامج [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) تأكد أيضا من تمكين الحصول الفردي Office الإضافية 'لمتجر'. 

1. تأكد من أن بيئتك تلبي متطلبات نشر الوظائف الإضافية باستخدام النشر المركزي. للحصول على التفاصيل، راجع [المتطلبات](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).
2. انتقل إلى **الإعدادات** المتكاملة الحصول على التطبيقات في Microsoft 365 مركز الإدارة لنشر  >    >   الوظائف الإضافية. 

ملاحظات: 

- تتطلب التطبيقات المتكاملة أن يكون المسؤول لديه أذونات المسؤول Exchange العام.

- عند نشر الوظائف الإضافية لمستخدمين متعددين، نوصي بإجراء التعيينات باستخدام المجموعات بدلا من المستخدمين الفرديين. للحصول على التفاصيل، راجع [الاعتبارات عند تعيين](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)مهمة إضافية للمستخدمين والمجموعات .

- النشر المركزي لا يدعم المستخدمين في المجموعات المتداخلة أو المجموعات التي لديها مجموعات أصل. للحصول على التفاصيل، راجع [تعيينات المستخدم والمجموعة](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).

- تأكد من تمكين خدمة إدارة تطبيقات Microsoft 365 (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') للمستخدمين من تسجيل الدخول. للحصول على التفاصيل، راجع [تكوين خصائص التطبيق](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).

- إذا واجهت مشاكل في نشر الوظائف الإضافية باستخدام التطبيقات المتكاملة، فحاول النشر باستخدام [الوظائف الإضافية.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)

لمزيد من المعلومات، اطلع على:

[نشر الوظائف الإضافية في مركز الإدارة](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [إدارة الوظائف الإضافية في مركز الإدارة](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [استخدام Cmdlets للنشر المركزي في PowerShell لإدارة الوظائف الإضافية](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [نشر Office الإضافية باستخدام "النشر](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) المركزي" عبر Microsoft 365 مركز الإدارة 
 [استكشاف الأخطاء وإصلاحها: لا](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) يرى المستخدم الوظائف الإضافية 
 [استكشاف أخطاء المستخدم](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting) وإصلاحها باستخدام Office الإضافية