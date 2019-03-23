---
title: 1065 "الإهمال من البرنامج" الخارجي IP عنوان rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: 0def0a93c61ea762918f1c9e6edb2e9b04446851
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30777259"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="9323f-102">الإهمال التنظيمي نطاقات عناوين IP الصادرة</span><span class="sxs-lookup"><span data-stu-id="9323f-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="9323f-103">لقد اكتشفنا مشكلة محتملة مع المؤسسة الخاصة بك (إذا لم يتم تصحيحها بتاريخ 26 تشرين الأول/أكتوبر 2018) قد قطع تدفق البريد الداخلي أو وجهات خارجية.</span><span class="sxs-lookup"><span data-stu-id="9323f-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="9323f-104">كما أبلغ عنها سابقا، لتبسيط إدارة نطاق عناوين IP، ونحن تقوم بالدمج نطاقات عناوين IP حماية Exchange عبر إنترنت (التنظيمي) التي يتم استخدامها لإرسال وتلقى البريد خارج Office 365.</span><span class="sxs-lookup"><span data-stu-id="9323f-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365.</span></span> <span data-ttu-id="9323f-105">يشير تحليلنا إلى أن واحد أو أكثر من المصادر الخارجية البريد الإلكتروني أو الوجهات التي قمت بتكوينها في الروابط تدفق البريد لا يتم قبول الاتصالات من على IP عنوان نطاقات عرضها [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9323f-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="9323f-106">تعمل قبل 26 تشرين الأول/أكتوبر لضمان قبول هذه المصادر ووجهات الاتصالات ومن كافة [عناوين IP البرنامج نشر](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9323f-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="9323f-107">لمزيد من المعلومات حول هذا التغيير، الرجاء مراجعة وظائف مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="9323f-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="9323f-108">**ملاحظة**: إذا استخدمت مسبقاً IP أو عنوان URL النشر عبر HTML و XML و RSS للتحديثات نقطة النهاية، كما يجب ترحيل لخدمات الويب الجديدة لهذه الأنواع من التحديثات بشكل تلقائي.</span><span class="sxs-lookup"><span data-stu-id="9323f-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="9323f-109">لمزيد من المعلومات، راجع [Office 365 نقطة النهاية فئات وعنوان IP Office 365 وخدمه ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="9323f-109">For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

