---
title: تثبيت المكتب على خادم المحطة الطرفية - غير مرخص
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
ms.openlocfilehash: 6e952513679c9ac66f8de2b43d6d243cf17ff789
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010601"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office على خادم المحطة الطرفية

لنشر تطبيقات Microsoft 365 للمؤسسات على خادم Windows باستخدام خدمات سطح المكتب البعيد (RDS)، التي كانت تسمى سابقًا خدمات المحطة الطرفية:
  
- يجب أن يكون لديك اشتراك Microsoft 365 يتضمن تطبيقات Microsoft 365 للمؤسسات، مثل Office 365 Enterprise E3 أو Enterprise E5. لا تتضمن تطبيقات Microsoft 365 للأعمال وتطبيقات Microsoft 365 لخطط Premium للأعمال تطبيقات Microsoft 365 للمؤسسات.

- تحتاج إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

إذا كنت ترغب في تثبيت تطبيقات Microsoft 365 للمؤسسات على RDS من مركز إدارة Microsoft 365، ***والذي يستخدم إعدادات التثبيت الافتراضية،*** فاستخدم الخطوات التالية.

> [!TIP]
> يمكنك أيضًا تنزيل [وتشغيل مساعد دعم واسترداد Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) لتثبيت تطبيقات Microsoft 365 للمؤسسات في وضع تنشيط الكمبيوتر المشترك.
  
1. تحقق من اشتراك Microsoft 365 لديك. [تعرف على كيفية](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. إذا لزم الأمر، قم بالتبديل إلى اشتراك Microsoft 365 مختلف. [تعرف على كيفية](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. إذا تم تثبيت Office بالفعل على خادم RDS باستخدام أي اشتراكات Microsoft 365 الأخرى، فقم بإلغاء تثبيته. على سبيل المثال، عن \> طريق الانتقال إلى لوحة التحكم إلغاء تثبيت برنامج. إلغاء التثبيت باستخدام [مساعد دعم Microsoft والاسترداد](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تقوم بمشكلات.

4. على خادم RDS، قم بتسجيل الدخول إلى مركز إدارة Microsoft 365 باستخدام حساب المسؤول [وتثبيت تطبيقات Microsoft 365 للمؤسسات](https://portal.office.com/OLS/MySoftware.aspx).

5. بعد تثبيت Office، ***لا تفتح أو تسجل الدخول*** إلى أي تطبيقات Office.

6. على ملقم RDS، تمكين تنشيط الكمبيوتر المشترك عن طريق تحرير التسجيل باتباع الخطوات التالية:

1. انقر بزر Windows في الزاوية اليسرى السفلى من الشاشة وحدد تشغيل. في المربع المفتوح، اكتب **regedit**، ثم حدد موافق.

2. حدد نعم عندما تتم مطالبتك بالسماح لمحرر التسجيل بإجراء تغييرات على جهازك.

3. في محرر التسجيل، قم بإضافة قيمة سلسلة من **SharedComputerLicensing** مع إعداد 1 تحت HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. على خادم RDS، ***قم بتسجيل الدخول كمستخدم نهائي*** وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft [365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

لمزيد من التفاصيل حول المتطلبات الأساسية وإرشادات الإعداد والإرشادات حول المنشآت المخصصة باستخدام أداة نشر Office، يرجى الاطلاع [على نشر تطبيقات Microsoft 365 للمؤسسات باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك، يرجى الاطلاع على [مشكلات استكشاف الأخطاء وإصلاحها المتعلقة بتنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 للمؤسسات](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  