---
title: موصل Intune في الداخل المحلي
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
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807212"
---
# <a name="intune-exchange-on-premise-connector"></a>موصل Intune في الداخل المحلي

للحصول علي تفاصيل حول اعداد الموصل بين Intune و Exchange الذي تتم استضافته محليا ، يرجى مراجعه الوثائق التالية:

[اعداد موصل Exchange المحلي في Intune في Microsoft Intune Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**الأسئلة المتداولة:**

س: اري خطا مثل "لا يتم اعتماد إصدار Exchange Connector" عند محاولة اعداد Exchange connector. "الاتصال". ما السبب في ذلك ؟

ج: الحساب الذي تستخدمه مرخص بشكل مناسب-يجب ان يتوفر لديه ترخيص Intune نشط

س: هل من الممكن ان يكون لديك عده موصلات في Exchange ؟

ج: يمكنك فقط اعداد موصل Exchange واحد لكل مؤسسه من المستاجرين في Exchange. يمكن تثبيت الموصل علي خادم واحد فقط في مؤسسه متعددة في exchange server.

كما لا يمكنك أيضا ان يكون لديك موصلات مكونه لكل من Exchange المحلي و Exchange Online التي تم تكوينها في المستاجر نفسه.

س: هل يستطيع الموصل استخدام صفيف CAS كاتصال ل Exchange ؟

ج: تحديد لا يمثل صفيف CAS تكوينا معتمدا في اعداد الموصل. يجب تحديد خادم واحد فقط ويجب ان يكون مضمن في ملف تكوين الموصل الذي يمكن العثور عليه في

برنامج data\microsoft\microsoft Intune علي اتصال Exchange connector المحلي \ OnpremiseExchangeConnectorServiceConfiguration.xml

حدد موقع الإدخال التالي ```<ExchangeWebServiceURL />``` واستبدل عنوان URL ب exchange server.

**مثال**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

يرجى مراجعه الوثائق التالية لاستكشاف الأخطاء وإصلاحها الاضافيه: [استكشاف الأخطاء في Exchange المحلي ل Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**تمكين التسجيل المطول لموصل Exchange**

1. افتح ملف تكوين تتبع الرابط في Exchange للتحرير.  
الملف موجود علي:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**مثال**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. حدد موقع تراسيسورسيليني مع المفتاح التالي: أونبريميسيسيكسكهانجيكونيكتورسيرفيسي  
  
3. تغيير قيمه عقده سورسيليفيل من المعلومات الأكتيفيتيتراسينج (الافتراضي) إلى الأكتيفيتيتراسينج المطول  

**مثال**
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
4. أعاده تشغيل خدمه Microsoft Intune Exchange  
5. مزامنة كامله في مدخل Intune حتى تنتهي ، ثم قم بتغيير XML مره أخرى إلى "معلومات أكتيفيتيتراسينج" ثم أعد تشغيل خدمه Microsoft Intune Exchange.  
6. موقع السجلات هو: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`