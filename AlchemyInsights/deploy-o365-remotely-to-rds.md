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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031465"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر Microsoft 365 Apps for enterprise للاستخدام المشترك على RDS أو Terminal Server أو VDI

لنشر الأجهزة Microsoft 365 Apps for enterprise خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقا خدمات المحطة الطرفية:

- يجب أن يكون لديك Microsoft 365 For Business أو خطة Office 365 تتضمن Microsoft 365 Apps for enterprise، مثل Office 365 Enterprise E3 أو Enterprise E5.
   > [!NOTE]
   > لا Microsoft 365 Apps for business الخطط Microsoft 365 Business Standard تتضمن Microsoft 365 Apps for enterprise.
- يجب تمكين تنشيط [الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> يمكنك أيضا تنزيل ملف [Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) مساعد الإصلاح والدعم عليه Microsoft 365 Apps for enterprise في وضع تنشيط الكمبيوتر المشترك.

لمزيد من المعلومات حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة النشر Office، راجع نشر Microsoft 365 Apps for enterprise باستخدام خدمات سطح المكتب [البعيد.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:

- راجع [استكشاف المشاكل المتعلقة بتنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)وإصلاحها Microsoft 365 Apps for enterprise .
- راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).

إذا كنت تريد تثبيت Microsoft 365 Apps for enterprise RDS من مركز مسؤولي Microsoft 365 الذي يستخدم إعدادات التثبيت الافتراضية، فاتبع الخطوات التالية:

1. تحقق من الاشتراك الذي تملكه. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. إذا لزم الأمر، قم بالتبديل إلى اشتراك آخر. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. إذا Office تم تثبيته بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft أخرى، ف إلغاء تثبيته. على سبيل المثال، عن طريق الذهاب إلى **لوحة التحكم** إلغاء  >  **تثبيت برنامج**. إلغاء تثبيت استخدام [Microsoft مساعد الإصلاح والدعم](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تخوض مشاكل.
4. على خادم RDS، سجل الدخول إلى مركز مسؤولي Microsoft 365 باستخدام حساب المسؤول ثم [قم بتثبيت Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. بعد Office، ***لا*** تفتح أو سجل الدخول إلى أي Office أخرى.
6. على خادم RDS، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:
   1. انقر بزر الماوس الأيمن Windows في الزاوية السفلية اليمنى من الشاشة وحدد **تشغيل**. في المربع فتح، اكتب **regedit**، ثم حدد **موافق**.
   2. حدد **نعم** عند مطالبتك بالسماح لمحرر السجل بإجراء تغييرات على جهازك.
   3. في محرر السجل، أضف قيمة سلسلة **ل SharedComputerLicensing** بإعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. على خادم RDS، سجل الدخول كمستخدم وتحقق من تمكين تنشيط الكمبيوتر المشترك [Microsoft 365 Apps for enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded) 
