---
title: موصل Exchange Intune
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 744758739c2ca839823d2c8b440ed7b0d9dd4f06ebbb6f19fe52041a6710c4b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013951"
---
# <a name="intune-exchange-on-premise-connector"></a>موصل Exchange Intune

للحصول على تفاصيل حول إعداد الموصل بين Intune Exchange المستضافة في الموقع، الرجاء الاطلاع على الوثائق التالية:

[إعداد موصل Intune Exchange في Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**الأسئلة المتداولة:**

س: أرى خطأ مثل "Exchange موصل غير معتمد" عند محاولة إعداد Exchange موصل. ما السبب الذي يمكن أن يكون السبب؟

أ: الحساب الذي تستخدمه مرخص بشكل مناسب - يجب أن يكون لديه ترخيص Intune نشط

س: هل من الممكن الحصول على موصلات Exchange متعددة؟

أ: يمكنك إعداد موصل Exchange واحد فقط لكل مستأجر Intune لكل Exchange المؤسسة. يمكن تثبيت الموصل على خادم واحد فقط في مؤسسة تبادل خوادم متعددة.

كما لا يمكنك تكوين الموصلات لكل من Exchange أو Exchange Online في نفس المستأجر.

س: هل يمكن للموصل استخدام صفيف CAS كاتصاله Exchange؟

أ: تحديد صفيف CAS ليس تكوينا معتمدا في إعداد الموصل. يجب تحديد خادم واحد فقط ويجب أن يتم ترميزه في ملف تكوين الموصل الذي يمكن العثور عليه في

بيانات البرنامج\microsoft\microsoft Intune Exchange الموصل\ OnpremiseExchangeConnectorServiceConfiguration.xml

حدد موقع الإدخال التالي ```<ExchangeWebServiceURL />``` واستبدل عنوان URL بخادم exchange.

**مثال:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

الرجاء الاطلاع على الوثائق التالية للحصول على مزيد من استكشاف الأخطاء وإصلاحها: استكشاف الأخطاء وإصلاحها في [موصل Intune Exchange](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**تمكين التسجيل المطوِّل Exchange الموصل**

1. افتح ملف Exchange تكوين تتبع الموصل للتحرير.  
يقع الملف في : ٪ProgramData٪\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**مثال:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. حدد موقع TraceSourceLine باستخدام المفتاح التالي: OnPremisesExchangeConnectorService  
  
3. تغيير قيمة عقدة SourceLevel من "نشاط المعلومات" (الافتراضي) إلى "تعقب النشاط المطيل"  

**على سبيل المثال:**
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. إعادة تشغيل Microsoft Intune Exchange الخدمة  
5. قم بالمزامنة الكاملة في مدخل Intune حتى تنتهي ثم قم بتغيير XML مرة أخرى إلى "نشاط المعلومات" ثم أعد تشغيل Microsoft Intune Exchange الخدمة.  
6. موقع السجلات هو : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`