---
title: تثبيت office علي خادم محطه طرفيه-غير مرخص
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
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663104"
---
# <a name="installing-office-on-a-terminal-server"></a>تثبيت Office علي خادم محطه طرفيه

بالنسبة إلى نشر تطبيقات Microsoft 365 للمؤسسة علي Windows Server باستخدام خدمات سطح المكتب البعيد (RDS) ، المسمية السابق الخدمات الطرفية:
  
- يجب ان يتوفر لديك اشتراك Microsoft 365 يتضمن تطبيقات Microsoft 365 ل enterprise ، مثل Office 365 Enterprise E3 أو Enterprise E5. لا تشمل تطبيقات Microsoft 365 للاعمال وتطبيقات Microsoft 365 لخطط business Premium تطبيقات Microsoft 365 ل enterprise.

- أنت بحاجه إلى تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

إذا كنت تريد تثبيت تطبيقات Microsoft 365 ل enterprise علي RDS من Microsoft 365 admin center ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، فاستخدم الخطوات التالية.

> [!TIP]
> يمكنك أيضا تنزيل [مساعد الإصلاح والدعم من microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات microsoft 365 ل enterprise في وضع تنشيط الكمبيوتر المشترك.
  
1. تحقق من اشتراك Microsoft 365 لديك. [تعرف علي كيفيه](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. إذا لزم الأمر ، فقم بالتبديل إلى اشتراك آخر في Microsoft 365. [تعرف علي كيفيه](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. إذا كان Office مثبتا بالفعل علي خادم RDS باستخدام اي اشتراكات Microsoft 365 أخرى ، فقم بازاله تثبيته. علي سبيل المثال ، بالانتقال إلى "لوحه التحكم" \> إلغاء تثبيت برنامج. أزاله [التثبيت باستخدام مساعد الإصلاح والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل علي مشاكل.

4. في RDS server ، سجل دخولك إلى مركز أداره Microsoft 365 باستخدام حساب المسؤول الخاص بك وقم [بتثبيت تطبيقات Microsoft 365 ل enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. بعد تثبيت Office ، ***لا تقم بفتح اي من تطبيقات Office أو تسجيل الدخول*** اليه.

6. في RDS server ، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:

1. انقر بزر الماوس الأيمن في الزاوية السفلية اليمني من الشاشة وحدد تشغيل. في المربع فتح ، اكتب **regedit**، ثم حدد موافق.

2. حدد نعم عندما تتم مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.

3. في "محرر السجل" ، أضف قيمه سلسله **شاريدكومبوتيرليسينسينج** باعداد 1 تحت HKEY_LOCAL_MACHINE \software\microsoft \office\clicktorun\configuration.

7. في RDS server ، ***سجل دخولك كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

للحصول علي مزيد من التفاصيل حول المتطلبات الاساسيه ، قم باعداد الإرشادات والإرشادات علي التثبيتات المخصصة باستخدام أداه نشر Office ، الرجاء مراجعه [نشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك ، يرجى مراجعه [استكشاف الأخطاء وإصلاحها في تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  