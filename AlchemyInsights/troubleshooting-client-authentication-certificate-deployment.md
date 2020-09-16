---
title: استكشاف أخطاء نشر شهادات مصادقه العميل وإصلاحها
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
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658973"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="c34b8-102">استكشاف أخطاء نشر شهادات مصادقه العميل وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="c34b8-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="c34b8-103">يتم استخدام ملفات تعريف شهادات عميل نديس/سسيب و PKCS/PFX بشكل شائع بالاضافه إلى أنواع ملفات تعريف أخرى مثل Wifi و VPN والبريد الكتروني للسماح للمستخدمين بالمصادقة علي موارد الشركة.</span><span class="sxs-lookup"><span data-stu-id="c34b8-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="c34b8-104">عند ارتباط أنواع ملفات التعريف هذه بملف تعريف شهادة عميل ، فانه يعتمد علي النشر الناجح لهذا التشكيل الجانبي.</span><span class="sxs-lookup"><span data-stu-id="c34b8-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="c34b8-105">غالبا ما يتطلب اعداد البنية الاساسيه الاوليه والتكوين المقترن بملف تعريف شهادة العميل استكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="c34b8-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="c34b8-106">للحصول علي دليل مفصل خطوه بخطوه لاعداد موصل نديس وإرشادات استكشاف الأخطاء وإصلاحها لعزل المشاكل المتعلقة بنشر الشهادات ، راجع:</span><span class="sxs-lookup"><span data-stu-id="c34b8-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="c34b8-107">تكوين البنية الاساسيه لدعم سسيب مع Intune</span><span class="sxs-lookup"><span data-stu-id="c34b8-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="c34b8-108">نظره عامه حول استكشاف أخطاء ملفات تعريف شهادات سسيب وإصلاحها باستخدام Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c34b8-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="c34b8-109">استخدم البرامج النصية ل powershell المشار اليها للمساعدة في التحقق من التكوين.</span><span class="sxs-lookup"><span data-stu-id="c34b8-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="c34b8-110">للحصول علي مزيد من المعلومات ، راجع [البرامج النصية للتحقق من موصل الشهادة Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="c34b8-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="c34b8-111">**مشاكل أخرى شائعه**</span><span class="sxs-lookup"><span data-stu-id="c34b8-111">**Other common issues**</span></span>

<span data-ttu-id="c34b8-112">**عندما أحاول تثبيت موصل الشهادة Intune علي خادم نديس connector ، أتلقى الرسالة "تعذر التحقق من كلمه المرور في طلب الشهادة. ربما تم استخدامه بالفعل. احصل علي كلمه مرور جديده لإرسالها بهذا الطلب. "**</span><span class="sxs-lookup"><span data-stu-id="c34b8-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="c34b8-113">تعني هذه الرسالة انك تحتاج إلى تشغيل تثبيت موصل الشهادة كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="c34b8-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="c34b8-114">في بعض البيئات ، يجب ان تستخدم الخوادم التي يتم فيها تشغيل شهادة Intune خادم وكيل للاتصال ب Intune ، التالي يجب ان يستخدم موصل الشهادة وكيلا.</span><span class="sxs-lookup"><span data-stu-id="c34b8-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="c34b8-115">في بعض الحالات ، يتجاهل موصل نديس إعدادات الوكيل المكونة ، وقد يكون من الضروري تكوين إعدادات الوكيل اثناء التشغيل في سياق أمان LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="c34b8-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="c34b8-116">الحل هو تشغيل Internet Explorer كنظام وتكوين وكيل في IE.</span><span class="sxs-lookup"><span data-stu-id="c34b8-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="c34b8-117">بعد أعاده تشغيل خدمه Intune Connector ، يتصل موصل نديس ب Intune.</span><span class="sxs-lookup"><span data-stu-id="c34b8-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="c34b8-118">**لم تعد أجهزه المستخدم تتلقي شهادات سسيب من نديس.**</span><span class="sxs-lookup"><span data-stu-id="c34b8-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="c34b8-119">من الممكن ان تكون شهادة مصادقه العميل التي تم إصدارها إلى خادم نديس ، والتي تم تحديدها اثناء تثبيت موصل نديس ، قد انتهت أو مفقوده.</span><span class="sxs-lookup"><span data-stu-id="c34b8-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="c34b8-120">لحل هذه المشكلة:</span><span class="sxs-lookup"><span data-stu-id="c34b8-120">To resolve:</span></span> 
 
1. <span data-ttu-id="c34b8-121">أزاله تثبيت موصل نديس.</span><span class="sxs-lookup"><span data-stu-id="c34b8-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="c34b8-122">استخدم هذه التفاصيل لطلب مصادقه عميل جديد أو شهادة مصادقه الخادم:</span><span class="sxs-lookup"><span data-stu-id="c34b8-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="c34b8-123">اسم الموضوع: CN = fqdn خارجي</span><span class="sxs-lookup"><span data-stu-id="c34b8-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="c34b8-124">الاسم البديل للموضوع (مطلوب كليهما): DNS = fqdn خارجي ، DNS = fqdn داخلي</span><span class="sxs-lookup"><span data-stu-id="c34b8-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="c34b8-125">أعد تثبيت موصل نديس مع الشهادة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="c34b8-125">Reinstall the NDES connector with the new certificate.</span></span>