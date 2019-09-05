---
title: تثبيت المكتب على ملقم المحطة الطرفية - غير مرخص
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 53071224a7c33532d864cd70b84bf0e3cc6a992f
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36735376"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office على ملقم المحطة طرفية

لنشر Office 365 ProPlus على ملقم Windows باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقاً "الخدمات الطرفية":
  
- يجب أن يكون لديك خطة Office 365 التي تتضمن Office 365 ProPlus، مثل Office 365 المؤسسة E3 أو المؤسسة E5. لا تتضمن خطط Office 365 الأعمال وOffice 365 الأعمال بريميوم Office 365.

- تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

إذا كنت ترغب في تثبيت Office 365 ProPlus على RDS من مركز مسؤول Microsoft 365 ***الذي يستخدم إعدادات التثبيت الافتراضية***اتبع الخطوات التالية:
  
1. تحقق من خطة Office 365 لديك. [تعرّف على كيفية](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. إذا لزم الأمر، قم بالتبديل إلى خطة Office 365 مختلفة. [تعرّف على كيفية](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. إذا كان Office مثبتًا بالفعل على ملقم RDS باستخدام أي خطط Office 365 أخرى، فقم بإلغاء تثبيته. على سبيل المثال، عن \> طريق الانتقال إلى "لوحة التحكم" إلغاء تثبيت برنامج. إلغاء التثبيت باستخدام [مساعد الدعم والاسترداد لـ Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل على مشكلات.

4. على ملقم RDS، قم بتسجيل الدخول إلى مركز مسؤول Microsoft 365 مع حساب المسؤول الخاص بك [وتثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. بعد تثبيت Office، لا تقم بفتح أي تطبيقات Office ***أو تسجيل الدخول*** إليها.

6. على ملقم RDS تمكين تنشيط الكمبيوتر المشترك عن طريق تحرير التسجيل باتباع الخطوات التالية:

1. انقر بزر الماوس الأيمن فوق زر Windows في الركن الأيمن السفلي من الشاشة وحدد تشغيل. في المربع فتح ، اكتب **regedit**، ثم حدد موافق.

2. حدد نعم عند مطالبتك بالسماح لمحرر التسجيل بإجراء تغييرات على جهازك.

3. في "محرر التسجيل" إضافة قيمة سلسلة **SharedComputerLicensing** مع إعداد 1 ضمن HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. على ملقم RDS تسجيل ***الدخول كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

لمزيد من التفاصيل حول المتطلبات المسبقة وإرشادات الإعداد والإرشادات حول عمليات التثبيت المخصصة باستخدام أداة نشر Office، الرجاء [مراجعة نشر Office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد".](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services)
  
لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، الرجاء [استكشاف مشكلات تنشيط الكمبيوتر المشترك لـ Office 365 ProPlus وإصلاحها.](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus)
  