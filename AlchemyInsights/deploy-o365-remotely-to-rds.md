---
title: نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200660"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر تطبيقات Microsoft 365 للمؤسسات للاستخدام المشترك على RDS أو Terminal Server أو VDI

لنشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقا خدمات المحطة الطرفية:

- يجب أن يكون لديك خطة Microsoft 365 for Business أو خطة Office 365 تتضمن تطبيقات Microsoft 365 للمؤسسات، مثل Office 365 Enterprise E3 أو Enterprise E5.
   > [!NOTE]
   > لا تتضمن خطط Microsoft 365 Apps للأعمال و Microsoft 365 Business Standard تطبيقات Microsoft 365 للمؤسسات.
- يجب تمكين تنشيط [الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> يمكنك أيضا تنزيل مساعد الاسترداد والدعم [من Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات Microsoft 365 للمؤسسات في وضع تنشيط الكمبيوتر المشترك.

لمزيد من المعلومات حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة نشر Office، راجع نشر [تطبيقات Microsoft 365](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)للمؤسسات باستخدام خدمات سطح المكتب البعيد .

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:

- راجع استكشاف المشاكل المتعلقة بتنشيط الكمبيوتر المشترك وإصلاحها [لتطبيقات Microsoft 365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).

إذا كنت تريد تثبيت تطبيقات Microsoft 365 للمؤسسات على RDS من مركز إدارة Microsoft 365، الذي يستخدم إعدادات التثبيت الافتراضية، فاتبع الخطوات التالية:

1. تحقق من الاشتراك الذي تملكه. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. إذا لزم الأمر، قم بالتبديل إلى اشتراك آخر. [تعرف على كيفية](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. إذا كان Office مثبتا بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft أخرى، ف إلغاء تثبيته. على سبيل المثال، عن طريق الذهاب إلى **لوحة التحكم** إلغاء  >  **تثبيت برنامج**. إلغاء التثبيت باستخدام مساعد الاسترداد [والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تخوض مشاكل.
4. على خادم RDS، سجل الدخول إلى مركز إدارة Microsoft 365 باستخدام حساب المسؤول وثبت [تطبيقات Microsoft 365 للمؤسسات](https://portal.office.com/OLS/MySoftware.aspx).
5. بعد تثبيت ***Office، لا*** تفتح أو سجل الدخول إلى أي من تطبيقات Office.
6. على خادم RDS، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:
   1. انقر بزر الماوس الأيمن فوق زر Windows في الزاوية السفلية اليمنى من الشاشة وحدد **تشغيل**. في المربع فتح، اكتب **regedit**، ثم حدد **موافق**.
   2. حدد **نعم** عند مطالبتك بالسماح لمحرر السجل بإجراء تغييرات على جهازك.
   3. في محرر السجل، أضف قيمة سلسلة **ل SharedComputerLicensing** بإعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. على خادم RDS، سجل الدخول كمستخدم وتحقق من تمكين تنشيط الكمبيوتر المشترك  [لتطبيقات Microsoft 365 للمؤسسات.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
