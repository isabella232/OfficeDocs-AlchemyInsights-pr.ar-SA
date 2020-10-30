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
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="b940a-102">موصل Intune في الداخل المحلي</span><span class="sxs-lookup"><span data-stu-id="b940a-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="b940a-103">للحصول علي تفاصيل حول اعداد الموصل بين Intune و Exchange الذي تتم استضافته محليا ، يرجى مراجعه الوثائق التالية:</span><span class="sxs-lookup"><span data-stu-id="b940a-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="b940a-104">اعداد موصل Exchange المحلي في Intune في Microsoft Intune Azure</span><span class="sxs-lookup"><span data-stu-id="b940a-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="b940a-105">**الأسئلة المتداولة:**</span><span class="sxs-lookup"><span data-stu-id="b940a-105">**FAQ:**</span></span>

<span data-ttu-id="b940a-106">س: اري خطا مثل "لا يتم اعتماد إصدار Exchange Connector" عند محاولة اعداد Exchange connector. "الاتصال".</span><span class="sxs-lookup"><span data-stu-id="b940a-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="b940a-107">ما السبب في ذلك ؟</span><span class="sxs-lookup"><span data-stu-id="b940a-107">What could be the cause?</span></span>

<span data-ttu-id="b940a-108">ج: الحساب الذي تستخدمه مرخص بشكل مناسب-يجب ان يتوفر لديه ترخيص Intune نشط</span><span class="sxs-lookup"><span data-stu-id="b940a-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="b940a-109">س: هل من الممكن ان يكون لديك عده موصلات في Exchange ؟</span><span class="sxs-lookup"><span data-stu-id="b940a-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="b940a-110">ج: يمكنك فقط اعداد موصل Exchange واحد لكل مؤسسه من المستاجرين في Exchange.</span><span class="sxs-lookup"><span data-stu-id="b940a-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="b940a-111">يمكن تثبيت الموصل علي خادم واحد فقط في مؤسسه متعددة في exchange server.</span><span class="sxs-lookup"><span data-stu-id="b940a-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="b940a-112">كما لا يمكنك أيضا ان يكون لديك موصلات مكونه لكل من Exchange المحلي و Exchange Online التي تم تكوينها في المستاجر نفسه.</span><span class="sxs-lookup"><span data-stu-id="b940a-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="b940a-113">س: هل يستطيع الموصل استخدام صفيف CAS كاتصال ل Exchange ؟</span><span class="sxs-lookup"><span data-stu-id="b940a-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="b940a-114">ج: تحديد لا يمثل صفيف CAS تكوينا معتمدا في اعداد الموصل.</span><span class="sxs-lookup"><span data-stu-id="b940a-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="b940a-115">يجب تحديد خادم واحد فقط ويجب ان يكون مضمن في ملف تكوين الموصل الذي يمكن العثور عليه في</span><span class="sxs-lookup"><span data-stu-id="b940a-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="b940a-116">برنامج data\microsoft\microsoft Intune علي اتصال Exchange connector المحلي \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="b940a-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="b940a-117">حدد موقع الإدخال التالي ```<ExchangeWebServiceURL />``` واستبدل عنوان URL ب exchange server.</span><span class="sxs-lookup"><span data-stu-id="b940a-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="b940a-118">**مثال**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="b940a-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="b940a-119">يرجى مراجعه الوثائق التالية لاستكشاف الأخطاء وإصلاحها الاضافيه: [استكشاف الأخطاء في Exchange المحلي ل Intune](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="b940a-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="b940a-120">**تمكين التسجيل المطول لموصل Exchange**</span><span class="sxs-lookup"><span data-stu-id="b940a-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="b940a-121">افتح ملف تكوين تتبع الرابط في Exchange للتحرير.</span><span class="sxs-lookup"><span data-stu-id="b940a-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="b940a-122">الملف موجود علي:%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="b940a-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="b940a-123">**مثال**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="b940a-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="b940a-124">حدد موقع تراسيسورسيليني مع المفتاح التالي: أونبريميسيسيكسكهانجيكونيكتورسيرفيسي</span><span class="sxs-lookup"><span data-stu-id="b940a-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="b940a-125">تغيير قيمه عقده سورسيليفيل من المعلومات الأكتيفيتيتراسينج (الافتراضي) إلى الأكتيفيتيتراسينج المطول</span><span class="sxs-lookup"><span data-stu-id="b940a-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="b940a-126">**مثال**</span><span class="sxs-lookup"><span data-stu-id="b940a-126">**Example:**</span></span>
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
4. <span data-ttu-id="b940a-127">أعاده تشغيل خدمه Microsoft Intune Exchange</span><span class="sxs-lookup"><span data-stu-id="b940a-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="b940a-128">مزامنة كامله في مدخل Intune حتى تنتهي ، ثم قم بتغيير XML مره أخرى إلى "معلومات أكتيفيتيتراسينج" ثم أعد تشغيل خدمه Microsoft Intune Exchange.</span><span class="sxs-lookup"><span data-stu-id="b940a-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="b940a-129">موقع السجلات هو: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="b940a-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>