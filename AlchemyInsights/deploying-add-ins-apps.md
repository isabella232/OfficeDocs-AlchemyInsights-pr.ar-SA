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
ms.openlocfilehash: a878a35ba9b530ce22ca7c263d20bd942d6896a8
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233500"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a>نشر الوظائف الإضافية Microsoft 365 Apps

النشر المركزي هو الطريقة المستحسنة لنشر Office الإضافية للمستخدمين والمجموعات داخل مؤسستك. لنشر الوظائف الإضافية، اتبع الخطوات أدناه:

**ملاحظة:** لتثبيت الوظائف الإضافية Office كمستخدم فردي، راجع عرض الوظائف الإضافية وإدارتها وتثبيتها في برامج [Office.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d) تأكد أيضا من تمكين الحصول الفردي Office الإضافية 'لمتجر'. للحصول على التفاصيل، راجع منع تنزيلات الوظائف الإضافية عن طريق إيقاف تشغيل Office عبر جميع العملاء [(باستثناء Outlook).](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center?view=o365-worldwide#prevent-add-in-downloads-by-turning-off-the-office-store-across-all-clients-except-outlook)

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