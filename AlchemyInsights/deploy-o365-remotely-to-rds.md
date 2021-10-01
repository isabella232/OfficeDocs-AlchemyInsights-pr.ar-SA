---
title: نشر Microsoft 365 Apps for enterprise للاستخدام المشترك على RDS أو Terminal Server أو VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/01/2021
ms.locfileid: "60040993"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر Microsoft 365 Apps for enterprise للاستخدام المشترك على RDS أو Terminal Server أو VDI

لنشر Microsoft 365 Apps سطح المكتب البعيد (RDS)، التي كانت تعرف سابقا بالخدمات الطرفية، يجب:

- استخدم الإصلاح السهل لتمكين TLS 1.2 كافتراضي إذا كنت تقوم بتشغيل إصدار أقدم من Windows (على سبيل المثال، Windows 7 SP1، Windows Server 2008 R2). للحصول على تصحيح سهل والمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy)كبروتوكولات آمنة افتراضية في WinHTTP في Windows . 
- لديك خطة تتضمن Microsoft 365 Apps for enterprise (سابقا Office 365 Plus). على سبيل المثال، Office 365 E3 أو Microsoft 365 E5، أو أي خطة تتضمن إصدار سطح المكتب من Project أو Visio، مثل Project (النظام 3) أو Visio (النظام 2)، أو خطة Microsoft 365 Business Premium، التي تتضمن أيضا Microsoft 365 Apps for business.
- تمكين تنشيط الكمبيوتر المشترك. لمزيد من المعلومات، راجع [نظرة عامة حول تنشيط الكمبيوتر المشترك Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation).

**ملاحظة**: لتثبيت Microsoft 365 Apps في وضع تنشيط الكمبيوتر المشترك، قم بتنزيل [Microsoft](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds)مساعد الإصلاح والدعم. للحصول على تفاصيل حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات لتخصيص عمليات التثبيت باستخدام أداة النشر Office، راجع نشر Microsoft 365 Apps باستخدام خدمات سطح المكتب [البعيد.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، راجع:

- [استكشاف المشاكل المتعلقة بتنشيط الكمبيوتر المشترك وإصلاحها Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [إعادة Microsoft 365 Apps for enterprise التنشيط](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

إذا كنت تريد تثبيت Microsoft 365 Apps RDS من مركز مسؤولي Microsoft 365 الذي يستخدم إعدادات التثبيت الافتراضية، فاتبع الخطوات التالية:

1. تحقق من Microsoft 365 لديك. لمزيد من المعلومات، راجع [ما هو الاشتراك الذي لدي؟](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. إذا لزم الأمر، قم بالتبديل إلى خطة Microsoft 365 أخرى. لمزيد من المعلومات، راجع [الترقية إلى خطة مختلفة](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. إذا Microsoft 365 Apps تم تثبيته بالفعل على خادم RDS باستخدام أي خطط أخرى غير متوافقة، ف إلغاء تثبيته عن طريق الذهاب إلى لوحة التحكم إلغاء   >  **تثبيت برنامج**. إذا كنت تخوض مشاكل، ف قم ب إلغاء التثبيت عن طريق تنزيل [Microsoft مساعد الإصلاح والدعم](https://aka.ms/SARA-OfficeUninstall-Alchemy).

1. على خادم RDS، سجل الدخول إلى مركز مسؤولي Microsoft 365 باستخدام حساب المسؤول ثم [قم بتثبيت Office](https://portal.office.com/OLS/MySoftware.aspx).

   بعد Office، لا تفتح أو سجل الدخول إلى أي Office أخرى.

1. على خادم RDS، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل:

   1. انقر بزر الماوس الأيمن Windows في الزاوية السفلية اليمنى من الشاشة وحدد **تشغيل**. في المربع فتح، اكتب **regedit**، ثم حدد **موافق**.

   1. عند مطالبتك بالسماح لمحرر السجل بإجراء تغييرات على جهازك، حدد **نعم**.

   1. في محرر السجل، ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration، أضف قيمة سلسلة **ل SharedComputerLicensing** بإعداد **1** .

1. على خادم RDS، سجل الدخول كمستخدم وتحقق من تمكين تنشيط الكمبيوتر المشترك Microsoft 365 Apps. 

   للحصول على التفاصيل، راجع التحقق من تمكين تنشيط الكمبيوتر [المشترك Microsoft 365 Apps](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).