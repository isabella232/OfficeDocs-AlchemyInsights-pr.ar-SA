---
title: المشاكل المتعلقة ب VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970966"
---
# <a name="vpn-related-issues"></a>المشاكل المتعلقة ب VPN

يعتمد التنفيذ الناجح لاتصال VPN لعملاء MDM على ملف تعريف تم نشره يعكس بشكل صحيح متطلبات البنية الأساسية ل VPN. للحصول على الإعدادات المناسبة ل الأنظمة الأساسية للعميل التي تقوم بالتحري بشأنها، راجع: 

[Windows 10 إعدادات Windows Holographic لإضافة اتصالات VPN باستخدام Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[إضافة إعدادات VPN على أجهزة iOS وiPadOS في Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[إعدادات جهاز Android لتكوين VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[إضافة إعدادات VPN على أجهزة macOS في Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

إذا كان ملف تعريف VPN يستخدم المصادقة المستندة إلى الشهادة، فتأكد من نشر ملفات تعريف شهادة الجذر ومصادقة العميل المرتبطة بملف تعريف VPN بنجاح.

**المشاكل الشائعة**

**لقد نشرت ملف تعريف VPN على جهاز. يظهر Intune نجاحه، ولكن الجهاز لا يتصل ب VPN.**

تعني الحالة الناجحة أن Intune قد نشر ملف التعريف بنجاح كما تم تكوينه. ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. راجع السجلات في البنية الأساسية وخدمة المصادقة (على خادم VPN وخادم NPS/نصف القطر) للحصول على مزيد من التفاصيل حول الاتصال الذي تم محاولة الاتصال به. قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مورد VPN من جهة خارجية، لجمع السجلات ومراجعتها.

**عند تكوين VPN مخصص ل iOS، لا يتم جعل ميزة VPN لكل تطبيق متوفرة.**

يتوفر VPN لكل تطبيق للأجهزة التي تعمل ب iOS في Intune حاليا لقائمة معينة من الموفرين والشركاء، الذين يجب عليهم أيضا تلبية المتطلبات الأساسية للشهادة قبل تكوين VPN لكل تطبيق. لمزيد من المعلومات، راجع إعداد الشبكة الخاصة الظاهرية (VPN) لكل تطبيق للأجهزة [التي تعمل ب iOS/iPadOS في Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

لمزيد من المعلومات حول كل أنواع اتصال VPN في Intune، راجع إنشاء ملفات تعريف VPN للاتصال خوادم [VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**لا يتم تشغيل iOS On-Demand VPN عند الوصول إلى مجال تم تكوينه**

لاختبار إعدادات VPN التلقائية، قم بتعيين القيم التالية:

أريد إجراء ما يلي: **تقييم كل محاولة اتصال** 

اختر ما إذا كنت تريد الاتصال: **الاتصال إذا لزم الأمر**

عند وصول المستخدمين إلى هذه المجالات: **اسم** *المجال الهدف*

إذا لم ينجح التكوين أعلاه، أضف العنصر التالي:

عندما يكون عنوان URL هذا غير قابل للوصول، يجبر على توصيل VPN: **BADURL**