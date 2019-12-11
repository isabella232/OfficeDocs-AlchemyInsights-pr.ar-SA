---
title: نشر Office 365 ProPlus للاستخدام المشترك علي RDS أو ملقم المحطة الطرفية أو VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959447"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر Office 365 ProPlus للاستخدام المشترك علي RDS أو ملقم المحطة الطرفية أو VDI

لنشر Office 365 ProPlus باستخدام خدمات سطح المكتب البعيد (RDS) ، المسمية سابقا "الخدمات الطرفية":
- يجب ان يكون لديك Microsoft 365 لخطه العمل أو خطه Office 365 التي تتضمن Office 365 ProPlus ، مثل Office 365 المؤسسة E3 أو المؤسسة E5.
   > [!NOTE] 
   > لا تتضمن خطط office 365 الاعمال والمكتب 365 Premium الاعمال Office 365 ProPlus.
- يجب تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> يمكنك أيضا تحميل وتشغيل [مساعد الدعم والاسترداد ل Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت Office 365 proplus في وضع تنشيط الكمبيوتر المشترك.

لمزيد من المعلومات حول المتطلبات الاساسيه وإرشادات الاعداد وإرشادات حول عمليات التثبيت المخصصة باستخدام أداه نشر Office ، راجع [نشر office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)".

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:
- راجع [استكشاف المشكلات وإصلاحها مع تنشيط الكمبيوتر المشترك ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- راجع [أعاده تعيين حاله تنشيط ProPlus ل Office 365](https://go.microsoft.com/fwlink/?linkid=2109218).

إذا كنت ترغب في تثبيت Office 365 ProPlus علي RDS من مركز مسؤول Microsoft 365 ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، اتبع الخطوات التالية:

1.  تحقق من خطه Office 365 التي لديك. [تعلم كيف](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have).
2.  إذا لزم الأمر ، قم بالتبديل إلى خطه 365 Office مختلفه. [تعلم كيف](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan).
3.  إذا كان Office مثبتا بالفعل علي ملقم RDS باستخدام إيه خطط Office 365 أخرى ، إلغاء تثبيته. علي سبيل المثال ، عن طريق الانتقال إلى >  **لوحه التحكم****إلغاء تثبيت برنامج**. إلغاء [التثبيت باستخدام دعم Microsoft ومساعد الاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت قيد التشغيل في المشكلات.
4.  علي ملقم RDS تسجيل الدخول إلى مركز مسؤول Microsoft 365 مع حساب المسؤول [وتثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  بعد تثبيت Office ، ***لا تقم بفتح أو تسجيل*** الدخول إلى اي من تطبيقات office.
6.  علي ملقم RDS تمكين تنشيط الكمبيوتر المشتركة عن طريق تحرير التسجيل باتباع الخطوات التالية:
   1. انقر نقرا ايمن فوق زر Windows في الزاوية السفلية اليسرى من الشاشة وحدد **تشغيل**. في المربع فتح ، اكتب **regedit**، ثم حدد **موافق**.
   2. حدد **نعم** عند المطالبة بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.
   3. في "محرر التسجيل" ، أضافه قيمه سلسله من **Sharedالكمبيوادالترخيص** مع اعداد من 1 ضمن HKEY_LOCAL_MACHINE \ البرنامج النصي \ Microsoft \Wic\clortorun\contate.
   4. علي ملقم RDS ***تسجيل الدخول كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشتركة ل Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

