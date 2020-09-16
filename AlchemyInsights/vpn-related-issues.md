---
title: المشاكل ذات الصلة ب VPN
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
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726078"
---
# <a name="vpn-related-issues"></a>المشاكل ذات الصلة ب VPN

يعتمد التنفيذ الناجح لاتصال VPN لعملاء MDM علي ملف تعريف منشور يعكس بشكل صحيح متطلبات البنية الاساسيه ل VPN. للحصول علي الإعدادات المناسبة للانظمه العميلة التي تقوم بالتحقق منها ، راجع: 

[إعدادات جهاز windows 10 و Windows هولوجرافيك لأضافه اتصالات VPN باستخدام Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[أضافه إعدادات VPN علي أجهزه iOS و إيبادوس في Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[إعدادات جهاز Android لتكوين VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[أضافه إعدادات VPN علي أجهزه macOS في Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

إذا كان ملف تعريف VPN الخاص بك يستخدم مصادقه مستنده إلى الشهادة ، فتاكد من ان الشهادة الجذر وملفات تعريف شهادة مصادقه العميل المرتبطة بملف تعريف VPN تم نشرها بنجاح.

**المشاكل الشائعة**

**لقد قمت بنشر ملف تعريف VPN إلى جهاز. يعرض Intune انه نجح ، ولكن الجهاز لا يتصل بشبكه VPN.**

تعني الحالة ناجح ان يقوم Intune بنشر ملف التعريف كما تم تكوينه بنجاح. ومع ذلك ، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. راجع السجلات في البنية الاساسيه وخدمه المصادقة (علي خادم VPN وخادم NPS/Radius) للحصول علي مزيد من التفاصيل حول الاتصال الذي تمت محاولته. قد تحتاج إلى العمل علي فريق البنية الاساسيه للشبكة ، أو مورد VPN التابع لجهة خارجيه ، لجمع السجلات ومراجعتها.

**عندما أقوم بتكوين VPN مخصص لنظام التشغيل iOS ، لم يتم توفير ميزه الإصدار VPN لكل تطبيق.**

يتوفر حاليا لكل تطبيق للاجهزه التي تعمل بنظام التشغيل iOS في Intune لقائمه معينه من الموفرين والشركاء ، الذين يجب أيضا ان يلبيوا متطلبات الشهادة قبل تكوين VPN لكل تطبيق. للحصول علي مزيد من المعلومات ، راجع اعداد [شبكه الاتصال الظاهرية الخاصة بكل تطبيق (VPN) لأجهزه iOS/إيبادوس في Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

للحصول علي مزيد من المعلومات حول كل أنواع اتصالات VPN في Intune ، راجع [إنشاء ملفات تعريف VPN للاتصال بخوادم VPN في intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**لا يتم تشغيل iOS عند الطلب في الشبكة**

لاختبار إعدادات VPN التلقائية ، قم بتعيين القيم التالية:

أريد القيام بما يلي: **تقييم كل محاولة اتصال** 

اختيار ما إذا كنت تريد الاتصال: **الاتصال عند الحاجة**

عندما يصل المستخدمون إلى هذه المجالات: *اسم المجال* **الهدف**

إذا لم ينجح التكوين أعلاه ، فأضف العنصر التالي:

عند تعذر الوصول إلى عنوان URL هذا ، قم بفرض توصيل VPN: **بادورل**