---
title: استكشاف أخطاء نشر شهادة مصادقة العميل
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2020
ms.locfileid: "46554719"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="2cfe7-102">استكشاف أخطاء نشر شهادة مصادقة العميل</span><span class="sxs-lookup"><span data-stu-id="2cfe7-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="2cfe7-103">إنتوني NDES / SCEP و PKCS / PFX ملفات تعريف شهادات العملاء تستخدم عادة جنبا إلى جنب مع أنواع التشكيلات الأخرى مثل واي فاي ، VPN ، والبريد الإلكتروني للسماح للمستخدمين بالمصادقة على موارد الشركات.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="2cfe7-104">عندما ترتبط أنواع ملفات التعريف هذه بملف تعريف شهادة العميل تعتمد على النشر الناجح لهذا التشكيل الجانبي.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="2cfe7-105">يتطلب إعداد البنية الأساسية الأولية والتكوين المقترن به لملف تعريف "شهادة العميل" غالباً استكشاف الأخطاء وإصلاحها.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="2cfe7-106">للحصول على دليل خطوة بخطوة للإعداد الناجح للموصل NDES والإرشاد لاستكشاف الأخطاء وإصلاحها لعزل المشكلات المتعلقة بنشر الشهادة، راجع:</span><span class="sxs-lookup"><span data-stu-id="2cfe7-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="2cfe7-107">تكوين البنية التحتية لدعم SCEP مع Intune</span><span class="sxs-lookup"><span data-stu-id="2cfe7-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="2cfe7-108">نظرة عامة لاستكشاف أخطاء SCEP الشهادات مع Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2cfe7-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="2cfe7-109">استخدم البرامج النصية powershell المرجعية للمساعدة في التحقق من التكوين.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="2cfe7-110">لمزيد من المعلومات، راجع [البرامج النصية للتحقق من موصل شهادة Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="2cfe7-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="2cfe7-111">**مسائل مشتركة أخرى**</span><span class="sxs-lookup"><span data-stu-id="2cfe7-111">**Other common issues**</span></span>

<span data-ttu-id="2cfe7-112">**عند محاولة تثبيت موصل شهادة إينتوني على ملقم موصل NDES، أحصل على الرسالة ، "لا يمكن التحقق من كلمة المرور في طلب الشهادة. ربما تم استخدامه بالفعل. الحصول على كلمة مرور جديدة لإرسالها مع هذا الطلب."**</span><span class="sxs-lookup"><span data-stu-id="2cfe7-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="2cfe7-113">تعني هذه الرسالة أنك تحتاج إلى تشغيل تثبيت موصل الشهادة كمسؤول.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="2cfe7-114">في بعض البيئات، يجب استخدام الملقمات حيث يتم تشغيل "شهادة إينتوني" ملقم وكيل للاتصال إينتوني، وبذلك يجب استخدام "رابط الشهادة" وكيل.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="2cfe7-115">في بعض الحالات، يتجاهل موصل NDES إعدادات الوكيل المكونة، وقد يكون من الضروري تكوين إعدادات الوكيل أثناء التشغيل في سياق الأمان LocalSystem.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="2cfe7-116">الحل هو تشغيل Internet Explorer كـ SYSTEM وتكوين وكيل في IE.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="2cfe7-117">بعد إعادة تشغيل خدمة رابط إينتوني، يتصل موصل NDES بـ Intune.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="2cfe7-118">**لم تعد أجهزة المستخدم تتلقى شهادات SCEP من NDES.**</span><span class="sxs-lookup"><span data-stu-id="2cfe7-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="2cfe7-119">من الممكن أن انتهت مدة صلاحية شهادة "مصادقة العميل" التي تم إصدارها إلى ملقم NDES، والمحددة أثناء تثبيت موصل NDES، أو مفقودة.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="2cfe7-120">لحل:</span><span class="sxs-lookup"><span data-stu-id="2cfe7-120">To resolve:</span></span> 
 
1. <span data-ttu-id="2cfe7-121">إلغاء تثبيت موصل NDES.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="2cfe7-122">استخدم هذه التفاصيل لطلب مصادقة عميل جديد أو شهادة مصادقة ملقم جديد:</span><span class="sxs-lookup"><span data-stu-id="2cfe7-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="2cfe7-123">اسم الموضوع: CN = fqdn الخارجية</span><span class="sxs-lookup"><span data-stu-id="2cfe7-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="2cfe7-124">اسم بديل الموضوع (كلاهما مطلوب): DNS = fqdn خارجي، DNS = fqdn الداخلية</span><span class="sxs-lookup"><span data-stu-id="2cfe7-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="2cfe7-125">أعد تثبيت موصل NDES مع الشهادة الجديدة.</span><span class="sxs-lookup"><span data-stu-id="2cfe7-125">Reinstall the NDES connector with the new certificate.</span></span>