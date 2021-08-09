---
title: 'ماسح ضوئي AIP: التثبيت والتكوين'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934244"
---
# <a name="aip-scanner-installation-and-configuration"></a>ماسح ضوئي AIP: التثبيت والتكوين

**لتثبيت ماسح AIP الضوئي، اتبع الإرشادات الموصى بها:**

1. إذا كنت تقوم بالترقية ولا تقوم بإجراء تثبيت نظيف، فالرجاء التأكد من أنك اتبعت إرشادات ترقية ماسح حماية المعلومات [من Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) ولعميل التسمية الموحد، راجع ترقية ماسح حماية المعلومات من [Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. تحقق من امتثالك لجميع متطلبات إعدادات جدران الحماية والبنية الأساسية [للشبكة](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. تأكد من [تعيين النهج إلى](https://docs.microsoft.com/azure/information-protection/configure-policy) تسمية تلقائية أو وضع تسمية افتراضية لها في النهج.
4. تأكد من تكوين نوع الملف ذي الصلة للتسمية/الحماية كما هو موضح في أنواع الملفات المعتمدة [بواسطة عميل Azure Information Protection](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). بالإضافة إلى ذلك، إذا كنت تريد تغيير السلوك الافتراضي، فاتبع الإرشادات التالية: تغيير مستوى الحماية [الافتراضي للملفات](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. تحقق من أن حساب المستخدم الذي تم تكوينه لتشغيل خدمة الماسح الضوئي لديه أذونات للوصول إلى كل المستودعات التي تم تكوينها.
6. إذا ما زلت تواجه مشاكل، فيرجى تصدير سجلات الماسح الضوئي وإضافتها إلى تذكرة الدعم.

**تصدير سجلات ماسح حماية المعلومات في Azure**

1. انتقل إلى ٪localappdata٪\Microsoft\MSIP ضمن سياق المستخدم الذي يقوم بتشغيل خدمة الماسح الضوئي.
2. اضغط على كل المحتويات ضمن مجلد MSIP.
3. احفظ السجلات إلى اختيارك للموقع، وأرفقها بطلب الخدمة.
4. يمكنك أيضا استخدام [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**لمزيد من المعلومات، راجع:**
- [نشر ماسح حماية المعلومات من Azure لتصنيف الملفات وحمايتها تلقائيا](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [تحديد المعلمة Token ل Set-AIPAuthentication واستخدامها](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [تشغيل دورة اكتشاف وعرض التقارير للماسح الضوئي](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [مراجعة وثائق Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [متطلبات حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [تنزيل عميل Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
