---
title: تثبيت office علي ملقم المحطة الطرفية-غير مرخص
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "37205396"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office علي ملقم المحطة الطرفية

لنشر Office 365 ProPlus علي ملقم Windows باستخدام خدمات سطح المكتب البعيد (RDS) ، المسمية سابقا "الخدمات الطرفية":
  
- يجب ان يكون لديك خطه 365 Office التي تتضمن Office 365 ProPlus ، مثل Office 365 المؤسسة E3 أو المؤسسة E5. لا تتضمن خطط office 365 الاعمال والمكتب 365 Premium الاعمال Office 365 ProPlus.

- تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

إذا كنت ترغب في تثبيت Office 365 ProPlus علي RDS من مركز مسؤول Microsoft 365 ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، اتبع الخطوات التالية.

> [!TIP]
> يمكنك أيضا تحميل وتشغيل [مساعد الدعم والاسترداد ل Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت Office 365 proplus في وضع تنشيط الكمبيوتر المشترك.
  
1. تحقق من خطه Office 365 التي لديك. [تعرف علي كيفيه](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. إذا لزم الأمر ، قم بالتبديل إلى خطه 365 Office مختلفه. [تعرف علي كيفيه](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. إذا كان Office مثبتا بالفعل علي ملقم RDS باستخدام إيه خطط Office 365 أخرى ، إلغاء تثبيته. علي سبيل المثال ، عن طريق الانتقال إلى "لوحه التحكم" \> إلغاء تثبيت برنامج. إلغاء [التثبيت باستخدام دعم Microsoft ومساعد الاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت قيد التشغيل في المشكلات.

4. علي ملقم RDS تسجيل الدخول إلى مركز مسؤول Microsoft 365 مع حساب المسؤول [وتثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. بعد تثبيت Office ، ***لا تقم بفتح أو تسجيل*** الدخول إلى اي من تطبيقات office.

6. علي ملقم RDS تمكين تنشيط الكمبيوتر المشتركة عن طريق تحرير التسجيل باتباع الخطوات التالية:

1. انقر نقرا ايمن فوق زر Windows في الزاوية السفلية اليمني من الشاشة وحدد تشغيل. في المربع فتح ، اكتب **regedit**، ثم حدد موافق.

2. حدد نعم عند مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.

3. في "محرر التسجيل" ، أضافه قيمه سلسله من **Sharedالكمبيوادالترخيص** مع اعداد من 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Date\clortorun\contate.

7. علي ملقم RDS ***تسجيل الدخول كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشتركة ل Office 365 proplus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

لمزيد من التفاصيل حول المتطلبات الاساسيه ، إرشادات الاعداد وإرشادات حول عمليات التثبيت المخصصة باستخدام أداه نشر Office ، الرجاء مراجعه [نشر office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)".
  
لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشتركة ، الرجاء مراجعه [استكشاف المشكلات وإصلاحها مع تنشيط الكمبيوتر المشترك ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  