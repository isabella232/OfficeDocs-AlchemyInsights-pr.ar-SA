---
title: تثبيت Office على خادم المحطة الطرفية - غير مرخص
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58321986"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office على خادم المحطة الطرفية

لنشر Microsoft 365 Apps for enterprise على خادم Windows سطح المكتب البعيد (RDS)، المسمى سابقا خدمات المحطة الطرفية:
  
- يجب أن يكون لديك Microsoft 365 يتضمن Microsoft 365 Apps for enterprise، مثل Office 365 Enterprise E3 أو Enterprise E5. لا Microsoft 365 Apps for business الخطط Microsoft 365 Apps for business Premium تتضمن Microsoft 365 Apps for enterprise.

- أنت بحاجة إلى تمكين [تنشيط الكمبيوتر المشترك.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

إذا كنت تريد تثبيت Microsoft 365 Apps for enterprise RDS من مركز مسؤولي Microsoft 365 الذي يستخدم إعدادات التثبيت ***الافتراضية،*** فاتبع الخطوات التالية.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. تحقق من Microsoft 365 اشتراكك. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. إذا لزم الأمر، قم بالتبديل إلى اشتراك Microsoft 365 آخر. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. إذا Office تم تثبيته بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft 365 أخرى، ف إلغاء تثبيته. على سبيل المثال، عن طريق الذهاب إلى لوحة التحكم \> إلغاء تثبيت برنامج. يمكنك إلغاء التثبيت باستخدام [Microsoft مساعد الإصلاح والدعم](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تخوض مشاكل.

4. على خادم RDS، سجل الدخول إلى مركز مسؤولي Microsoft 365 باستخدام حساب المسؤول ثم [قم بتثبيت Microsoft 365 Apps for enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. بعد Office، لا تفتح أو ***سجل*** الدخول إلى أي Office أخرى.

6. على خادم RDS، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:

1. انقر بزر الماوس الأيمن Windows في الزاوية السفلية اليمنى من الشاشة وحدد تشغيل. في المربع فتح، اكتب **regedit**، ثم حدد موافق.

2. حدد نعم عند مطالبتك بالسماح لمحرر السجل بإجراء تغييرات على جهازك.

3. في محرر السجل، أضف قيمة سلسلة **ل SharedComputerLicensing** بإعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. على خادم RDS، سجل الدخول كمستخدم وتحقق من تمكين تنشيط الكمبيوتر المشترك [Microsoft 365 Apps for enterprise.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded) 

للحصول على مزيد من التفاصيل حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة النشر Office، الرجاء الاطلاع على نشر Microsoft 365 Apps for enterprise باستخدام خدمات سطح المكتب [البعيد.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، الرجاء الاطلاع على استكشاف أخطاء تنشيط الكمبيوتر المشترك وإصلاحها [Microsoft 365 Apps for enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  