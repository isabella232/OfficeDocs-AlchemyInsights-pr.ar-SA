---
title: مشكلات متعلقة بشبكة VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554711"
---
# <a name="vpn-related-issues"></a>مشكلات متعلقة بشبكة VPN

يعتمد التنفيذ الناجح لاتصال VPN لعملاء MDM على ملف تعريف تم نشره يعكس متطلبات البنية التحتية لـ VPN بشكل صحيح. للحصول على الإعدادات المناسبة للأنظمة الأساسية العميل الذي تقوم بالتحقق منها، راجع: 

[إعدادات الجهاز ثلاثي الأبعاد ويندوز ويندوز 10 لإضافة اتصالات VPN باستخدام Intune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[إضافة إعدادات VPN على أجهزة iOS وiPadOS في Microsoft Intune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[إعدادات جهاز أندرويد لتكوين VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-android)  
[إضافة إعدادات VPN على أجهزة macOS في Microsoft Intune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

إذا كان ملف تعريف VPN يستخدم مصادقة مستندة إلى الشهادة، تأكد من نشر شهادات الجذر و ملفات تعريف شهادة مصادقة العميل المرتبطة بملف تعريف VPN بنجاح.

**القضايا المشتركة**

**لقد قمت بنشر ملف تعريف VPN على جهاز. Intune يظهر أنه كان ناجحا، ولكن الجهاز لا يتصل VPN.**

حالة ناجحة يعني أن Intune نشر التشكيل الجانبي كما تم تكوينها بنجاح. ومع ذلك، قد لا تتطابق هذه التكوينات مع متطلبات الشبكة و/أو المصادقة. مراجعة سجلات في البنية التحتية وخدمة المصادقة (على ملقم VPN و NPS/ Radius الملقم) للحصول على مزيد من التفاصيل حول الاتصال محاولة. قد تحتاج إلى العمل مع فريق البنية الأساسية للشبكة، أو مع مورد VPN التابع لجهة خارجية، لجمع سجلات ومراجعةها.

**عند تكوين VPN مخصص لنظام iOS، لا يتم توفير ميزة الشبكة الافتراضية الخاصة لكل تطبيق.**

تتوفر حاليًا شبكة VPN لكل تطبيق لأجهزة iOS في Intune لقائمة محددة من مقدمي الخدمات والشركاء ، الذين يجب عليهم أيضًا تلبية متطلبات الشهادة قبل تكوين VPN لكل تطبيق. لمزيد من المعلومات، راجع [إعداد الشبكة الافتراضية الخاصة (VPN) لكل تطبيق لأجهزة iOS/iPadOS في Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

لمزيد من المعلومات حول كافة أنواع اتصالات VPN في Intune، راجع [إنشاء ملفات تعريف VPN للاتصال بخوادم VPN في Intune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**لا يتم تشغيل iOS عند الطلب VPN عند الوصول إلى مجال مكون**

لاختبار إعدادات VPN التلقائية، قم بتعيين القيم التالية:

أريد القيام بما يلي: **تقييم كل محاولة اتصال** 

اختر ما إذا كنت تريد الاتصال: **الاتصال إذا لزم الأمر**

عندما يقوم المستخدمون بالوصول إلى هذه المجالات: *اسم المجال* **الهدف**

إذا كان التكوين أعلاه غير ناجح، أضف العنصر التالي:

عندما يكون URL هذا غير قابل للوصول، قوة الاتصال VPN: **BADURL**