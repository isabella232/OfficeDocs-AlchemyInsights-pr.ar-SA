---
title: نشر تطبيقات Microsoft 365 ل enterprise for use المشتركة علي RDS أو الخادم الطرفي أو VDI
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: bd30d99221e3ddd0b07db0db78009f346babd2d0
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786264"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>نشر تطبيقات Microsoft 365 ل enterprise for use المشتركة علي RDS أو الخادم الطرفي أو VDI

لنشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد (RDS) ، المعروف سابقا بالخدمات الطرفية:
- يجب ان يتوفر لديك خطه Microsoft 365 For Business أو خطه Office 365 التي تتضمن تطبيقات Microsoft 365 ل enterprise ، مثل Office 365 Enterprise E3 أو Enterprise E5.
   > [!NOTE] 
   > لا تتضمن تطبيقات Microsoft 365 للاعمال وخطط Microsoft 365 Business Premium القياسية تطبيقات Microsoft 365 ل enterprise.
- يجب تمكين [تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> يمكنك أيضا تنزيل [مساعد الإصلاح والدعم من microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) وتشغيله لتثبيت تطبيقات microsoft 365 ل enterprise في وضع تنشيط الكمبيوتر المشترك.

للحصول علي مزيد من المعلومات حول المتطلبات الاساسيه وإرشادات الاعداد والإرشادات علي التثبيتات المخصصة باستخدام أداه نشر Office ، راجع [نشر تطبيقات Microsoft 365 للمؤسسة باستخدام خدمات سطح المكتب البعيد](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

لإصلاح الأخطاء المتعلقة بتنشيط الكمبيوتر المشترك:
- راجع [استكشاف الأخطاء وإصلاحها في تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- راجع [إعادة تعيين تطبيقات Microsoft 365 لحالة تفعيل المؤسسة](https://go.microsoft.com/fwlink/?linkid=2109218).

إذا كنت تريد تثبيت تطبيقات Microsoft 365 ل enterprise علي RDS من Microsoft 365 admin center ، ***الذي يستخدم إعدادات التثبيت الافتراضية***، فاستخدم الخطوات التالية:

1.    التحقق من الاشتراك الذي تملكه. [تعرف علي كيفيه القيام](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)بذلك.
2.    إذا لزم الأمر ، فقم بالتبديل إلى اشتراك مختلف. [تعرف علي كيفيه القيام](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)بذلك.
3.    إذا كان Office مثبتا بالفعل علي RDS server باستخدام اي اشتراكات Microsoft أخرى ، فقم بازاله تثبيته. علي سبيل المثال ، بالانتقال إلى **"لوحه التحكم"**  >  **إلغاء تثبيت برنامج**. أزاله [التثبيت باستخدام مساعد الإصلاح والدعم من Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) إذا كنت تعمل علي مشاكل.
4.    في RDS server ، سجل دخولك إلى مركز أداره Microsoft 365 باستخدام حساب المسؤول الخاص بك وقم [بتثبيت تطبيقات Microsoft 365 ل enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5.    بعد تثبيت Office ، ***لا تقم بفتح اي من تطبيقات Office أو تسجيل الدخول*** اليه.
6.    في RDS server ، قم بتمكين تنشيط الكمبيوتر المشترك عن طريق تحرير السجل باتباع الخطوات التالية:
   1. انقر بزر الماوس الأيمن فوق الشكل الموجود في الزاوية السفلية اليمني من الشاشة وحدد **تشغيل**. في المربع فتح ، اكتب **regedit**، ثم حدد **موافق**.
   2. حدد **نعم** عندما تتم مطالبتك بالسماح لمحرر التسجيل باجراء تغييرات علي جهازك.
   3. في "محرر السجل" ، أضف قيمه سلسله **شاريدكومبوتيرليسينسينج** باعداد 1 تحت HKEY_LOCAL_MACHINE \software\microsoft \office\clicktorun\configuration.
   4. في RDS server ، ***سجل دخولك كمستخدم نهائي*** [وتحقق من تمكين تنشيط الكمبيوتر المشترك لتطبيقات Microsoft 365 ل enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

