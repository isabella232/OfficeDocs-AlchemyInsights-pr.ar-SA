---
title: 'ماسح AIP: التثبيت والتكوين'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44357289"
---
# <a name="aip-scanner-installation-and-configuration"></a>ماسح AIP: التثبيت والتكوين

**لتثبيت ماسح AIP، اتبع الإرشادات الموصى بها:**

1. إذا كنت تقوم بالترقية ولا تقوم بإجراء تثبيت نظيف، يرجى التأكد من اتباع الإرشادات الخاصة [بترقية ماسح Azure لحماية المعلومات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) وعميل وضع العلامات الموحد، راجع [ترقية ماسح حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. تحقق من امتثالك لكافة [متطلبات جدران الحماية وإعدادات البنية التحتية للشبكة](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. تأكد من [تعيين النُهج](https://docs.microsoft.com/azure/information-protection/configure-policy) إلى وضع العلامات التلقائية أو أن يكون لها تسمية افتراضية في النهج.
4. تأكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في [أنواع الملفات التي يدعمها عميل حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). بالإضافة إلى ذلك، إذا كنت ترغب في تغيير السلوك الافتراضي، اتبع هذه الإرشادات: [تغيير مستوى الحماية الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. تحقق من أن حساب المستخدم الذي تم تكوينه لتشغيل خدمة الماسح الضوئي لديه أذونات للوصول إلى كافة المستودعات التي تم تكوينها.
6. إذا كنت لا تزال تواجه مشكلات، يرجى تصدير سجلات الماسح الضوئي وإضافتها إلى تذكرة الدعم الخاصة بك.

**تصدير سجلات الماسح الضوئي لحماية المعلومات Azure**

1. انتقل إلى %localappdata%\Microsoft\MSIP ضمن سياق المستخدم الذي يقوم بتشغيل خدمة الماسح الضوئي.
2. قم بإلغاء كافة المحتويات تحت مجلد MSIP.
3. احفظ السجلات على اختيارك للموقع، وإرفاقها بطلب الخدمة الخاص بك.
4. يمكنك أيضا استخدام [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**لمزيد من المعلومات، راجع:**
- [نشر ماسح حماية المعلومات Azure لتصنيف الملفات وحمايتها تلقائيًا](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [تحديد واستخدام معلمة الرمز المميز لمجموعة-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [تشغيل دورة اكتشاف وعرض تقارير للماسح الضوئي](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [مراجعة وثائق حماية المعلومات Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [متطلبات حماية المعلومات اللازوردية](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [تحميل عميل حماية المعلومات Azure](https://www.microsoft.com/download/details.aspx?id=53018)
