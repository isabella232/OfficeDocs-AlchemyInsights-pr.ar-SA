---
title: 1065 الإهمال من EOP الصادرة عنوان IP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: f4854c32d970d84f3a0664a9e384dc6e3cd0bfa7
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704584"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="7e555-102">إهمال نطاقات عنوان IP الصادرة EOP</span><span class="sxs-lookup"><span data-stu-id="7e555-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="7e555-103">لقد اكتشفنا مشكلة محتملة مع مؤسستك قد تكسر تدفق البريد إلى وجهاتك الداخلية أو الخارجية (إذا لم يتم تصحيحها بحلول 26 أكتوبر 2018).</span><span class="sxs-lookup"><span data-stu-id="7e555-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="7e555-104">كما تم إرساله مسبقًا ، لتبسيط إدارة نطاق عنوان IP ، نقوم بدمج نطاقات عنوان IP لحماية Exchange عبر الإنترنت (EOP) المستخدمة لإرسال واستقبال البريد الإلكتروني خارج Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="7e555-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="7e555-105">يشير تحليلنا إلى أن واحدًا أو أكثر من مصادر البريد الإلكتروني الخارجية أو الوجهات التي قمت بتكوينها في موصلات تدفق البريد لا تقبل الاتصالات من نطاقات عنوان IP الموضحة [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7e555-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7e555-106">العمل قبل 26 أكتوبر لضمان قبول هذه المصادر والوجهات الاتصالات من وإلى جميع [عناوين IP EOP المنشورة](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="7e555-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="7e555-107">لمزيد من المعلومات حول هذا التغيير، يرجى الاطلاع على منشورات مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="7e555-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="7e555-108">**ملاحظة:** إذا كنت تستخدم مسبقاً نشر IP أو URL عبر HTML و XML و RSS لتحديثات نقطة النهاية، فيجب عليك أيضًا الترحيل إلى خدمات الويب الجديدة لأتمتة هذه الأنواع من التحديثات.</span><span class="sxs-lookup"><span data-stu-id="7e555-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="7e555-109">لمزيد من المعلومات، راجع [فئات نقطة نهاية Microsoft 365 وعنوان IP Microsoft 365 وخدمة ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="7e555-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
