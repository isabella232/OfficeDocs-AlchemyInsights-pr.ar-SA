---
title: نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: ddd44d40e9430ee31b8b734450dde0defef229d7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704692"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI

لنشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقًا خدمات المحطة الطرفية:
- يجب أن يكون لديك خطة Microsoft 365 For Business أو خطة Office 365 التي تتضمن تطبيقات Microsoft 365 للمؤسسات، مثل Office 365 Enterprise E3 أو Enterprise E5.
   > [!NOTE] 
   > لا تتضمن تطبيقات Microsoft 365 للأعمال وخطط Microsoft 365 Business Premium Standard تطبيقات Microsoft 365 للمؤسسات.
- يجب تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> يمكنك أيضًا تنزيل [وتشغيل مساعد دعم واسترداد Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت تطبيقات Microsoft 365 للمؤسسات في وضع تنشيط الكمبيوتر المشترك.

لمزيد من المعلومات حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة نشر Office، راجع [نشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:
- راجع [استكشاف الأخطاء وإصلاحها مع تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).

إذا كنت ترغب في تثبيت تطبيقات Microsoft 365 للمؤسسات على RDS من مركز إدارة Microsoft 365، ***والذي يستخدم إعدادات التثبيت الافتراضية،*** فاستخدم الخطوات التالية:

1.    تحقق من الاشتراك الذي لديك. [تعرف على كيفية](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.    إذا لزم الأمر، قم بالتبديل إلى اشتراك مختلف. [تعرف على كيفية](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.    إذا تم تثبيت Office بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft أخرى، فقم بإلغاء تثبيته. على سبيل المثال، عن طريق الانتقال إلى **لوحة** > التحكم**إلغاء تثبيت برنامج**. إلغاء التثبيت باستخدام [مساعد دعم Microsoft والاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تقوم بمشكلات.
4.    على خادم RDS، قم بتسجيل الدخول إلى مركز إدارة Microsoft 365 باستخدام حساب المسؤول [وتثبيت تطبيقات Microsoft 365 للمؤسسات](https://portal.office.com/OLS/MySoftware.aspx).
5.    بعد تثبيت Office، ***لا تفتح أو تسجل الدخول*** إلى أي تطبيقات Office.
6.    على ملقم RDS، تمكين تنشيط الكمبيوتر المشترك عن طريق تحرير التسجيل باتباع الخطوات التالية:
   1. انقر بزر Windows في الزاوية اليسرى السفلى من الشاشة وحدد **تشغيل**. في المربع المفتوح، اكتب **regedit،** ثم حدد **موافق**.
   2. حدد **نعم** عندما تتم مطالبتك بالسماح لمحرر التسجيل بإجراء تغييرات على جهازك.
   3. في محرر التسجيل، قم بإضافة قيمة سلسلة من **SharedComputerLicensing** مع إعداد 1 تحت HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. على خادم RDS، ***قم بتسجيل الدخول كمستخدم نهائي*** وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft [365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

