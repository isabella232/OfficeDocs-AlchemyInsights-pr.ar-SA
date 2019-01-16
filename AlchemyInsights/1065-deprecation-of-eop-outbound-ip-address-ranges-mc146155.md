---
title: 1065 "الإهمال من البرنامج" الخارجي IP عنوان rangesMC146155
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: ec87141ffaa2fa3484620a9b52851e3e92f20b6b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273273"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7c27e-102">الإهمال التنظيمي نطاقات عناوين IP الصادرة</span><span class="sxs-lookup"><span data-stu-id="7c27e-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7c27e-p101">لقد اكتشفنا مشكلة محتملة مع المؤسسة الخاصة بك (إذا لم يتم تصحيحها بتاريخ 26 تشرين الأول/أكتوبر 2018) قد قطع تدفق البريد الداخلي أو وجهات خارجية. كما أبلغ عنها سابقا، لتبسيط إدارة نطاق عناوين IP، ونحن تقوم بالدمج نطاقات عناوين IP حماية Exchange عبر إنترنت (التنظيمي) التي يتم استخدامها لإرسال وتلقى البريد خارج Office 365. يشير تحليلنا إلى أن واحد أو أكثر من المصادر الخارجية البريد الإلكتروني أو الوجهات التي قمت بتكوينها في الروابط تدفق البريد لا يتم قبول الاتصالات من على IP عنوان نطاقات عرضها [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7c27e-p101">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations. As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Office 365. Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7c27e-106">تعمل قبل 26 تشرين الأول/أكتوبر لضمان قبول هذه المصادر ووجهات الاتصالات ومن كافة [عناوين IP البرنامج نشر](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7c27e-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
  
<span data-ttu-id="7c27e-107">لمزيد من المعلومات حول هذا التغيير، الرجاء مراجعة وظائف مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7c27e-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>
  
 <span data-ttu-id="7c27e-p102">**ملاحظة**: إذا استخدمت مسبقاً IP أو عنوان URL النشر عبر HTML و XML و RSS للتحديثات نقطة النهاية، كما يجب ترحيل لخدمات الويب الجديدة لهذه الأنواع من التحديثات بشكل تلقائي. لمزيد من المعلومات، راجع [Office 365 نقطة النهاية فئات وعنوان IP Office 365 وخدمه ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7c27e-p102">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates. For more information, see [Office 365 endpoint categories and Office 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
  

