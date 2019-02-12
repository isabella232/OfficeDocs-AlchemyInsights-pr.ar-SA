---
title: تثبيت office على "ملقم المحطة الطرفية"-غير مرخص
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918961"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office على ملقم المحطة الطرفية

لنشر Office 365 ProPlus على خادم Windows استخدام خدمات سطح المكتب البعيد (RDS)، المعروف فيما مضى "الخدمات الطرفية":
  
- يجب أن يكون لديك مخطط Office 365 يتضمن Office 365 ProPlus، مثل Office 365 المؤسسة E3 أو E5 المؤسسة. لا يتم تضمين خطط العمل 365 Office و Office 365 الأعمال الأولية Office 365 ProPlus.
    
- تحتاج إلى تمكين [تنشيط الكمبيوتر المشتركة](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
إذا أردت تثبيت Office 365 ProPlus على RDS من المدخل Office 365، * * *التي تستخدم إعدادات التثبيت الافتراضي* * *، اتبع الخطوات التالية: 
  
1. تحقق من خطة Office 365 ما لديك. [تعلم كيف](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. إذا لزم الأمر، قم بالتبديل إلى Office 365 مختلفة تخطط. [تعلم كيف](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. إذا كان Office مثبتاً على RDS server استخدام أي خطط Office 365، إلغاء تثبيته. على سبيل المثال، عن طريق الانتقال إلى "لوحة التحكم" \> بإلغاء تثبيت برنامج. إلغاء استخدام [دعم Microsoft ومساعد الاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تشغل في القضايا. 
    
4. على RDS server، تسجيل الدخول إلى موقع Office 365 باستخدام حساب المسؤول و [تثبيت Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. بعد تثبيت Office، * * *عدم فتح أو تسجيل الدخول* * * لأي من تطبيقات Office. 
    
6. على RDS server تمكين تنشيط الكمبيوتر المشترك بتحرير التسجيل باتباع الخطوات التالية:
    
1. انقر فوق الزر Windows في الزاوية السفلي اليسرى من الشاشة، وحدد تشغيل. في المربع فتح، اكتب **regedit**، ومن ثم حدد "موافق". 
    
2. حدد نعم عندما يطلب منك السماح "محرر التسجيل" لإجراء تغييرات على الجهاز الخاص بك.
    
3. في "محرر التسجيل"، إضافة قيمة سلسلة من **شاريدكومبوتيرليسينسينج** بإعداد 1 تحت HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. على RDS server * * *تسجيل الدخول كمستخدم نهائي* * * و [تحقق من أنه تم تمكين تنشيط الكمبيوتر المشتركة ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
لمزيد من التفاصيل حول المتطلبات المسبقة والإرشادات والتوجيهات بشأن عمليات التثبيت المخصص باستخدام أداة نشر Office، الرجاء مراجعة [توزيع Office 365 ProPlus باستخدام "خدمات سطح المكتب البعيد"](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
لحل الأخطاء المتعلقة بتنشيط الكمبيوتر المشتركة، راجع [استكشاف مشكلات تنشيط الكمبيوتر المشتركة ل Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

