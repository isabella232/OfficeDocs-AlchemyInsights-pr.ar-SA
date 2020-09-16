---
title: 'الماسح الضوئي ل IP: التثبيت والتكوين'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686629"
---
# <a name="aip-scanner-installation-and-configuration"></a>الماسح الضوئي ل IP: التثبيت والتكوين

**لتثبيت الماسح الضوئي AIP ، اتبع الإرشادات المستحسنة**:

1. إذا كنت تقوم بالترقية ولا تجري التثبيت النظيف ، فالرجاء التاكد من اتباع الإرشادات المتعلقة [بترقيه الماسح الضوئي لحماية البيانات في azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ولعميل التسمية الموحد ، راجع [ترقيه الماسح الضوئي لحماية البيانات في azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. تاكد من انك تلتزم بكل [متطلبات إعدادات الشبكات الاساسيه وجدران الحماية](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. تاكد من تعيين التسمية التلقائية [للنهج الخاصة](https://docs.microsoft.com/azure/information-protection/configure-policy) بك أو الحصول علي تسميات افتراضيه في النهج.
4. تاكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في [أنواع الملفات التي يعتمدها عميل حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). بالاضافه إلى ذلك ، إذا كنت تريد تغيير السلوك الافتراضي ، فاتبع الإرشادات التالية: [تغيير مستوي الحماية الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. تاكد من ان حساب المستخدم الذي تم تكوينه لتشغيل خدمه الماسح الضوئي يملك أذونات للوصول إلى كل المستودعات التي تم تكوينها.
6. إذا كنت لا تزال تواجه مشاكل ، يرجى تصدير سجلات الماسح الضوئي وأضافها إلى تذكره الدعم.

**تصدير سجلات الماسح الخاصة بحماية البيانات في Azure**

1. انتقل إلى%localappdata%\Microsoft\MSIP تحت سياق المستخدم الذي يقوم بتشغيل خدمه الماسح الضوئي.
2. الكل المحتويات أسفل المجلد مسيب.
3. احفظ السجلات في اختيار الموقع ، وقم بإرفاقها بطلب الخدمة.
4. يمكنك أيضا استخدام [التصدير-أيبلوجس-أونبيهالفوف](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**للحصول علي مزيد من المعلومات ، راجع**:
- [نشر الماسح الضوئي لحماية البيانات في Azure لتصنيف الملفات وحمايتها تلقائيا](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [تحديد معلمه الرمز المميز لأيباوثينتيكيشن واستخدامها](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [تشغيل دوره اكتشاف وعرض التقارير الخاصة بالماسح الضوئي](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [مراجعه وثائق حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [متطلبات حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [تنزيل عميل حماية المعلومات في Azure](https://www.microsoft.com/download/details.aspx?id=53018)
