---
title: 1065 إهمال عناوين IP الصادرة ل EOP rangesMC146155
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1065
ms.assetid: bd41784e-8002-428d-bc19-25671cfd34e8
ms.openlocfilehash: afd725668f906339f4b7d769bb67a4d2ee5a6ac6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806782"
---
# <a name="deprecation-of-eop-outbound-ip-address-ranges"></a><span data-ttu-id="611ad-102">نطاقات عناوين IP الصادرة ل EOP</span><span class="sxs-lookup"><span data-stu-id="611ad-102">Deprecation of EOP outbound IP address ranges</span></span>

<span data-ttu-id="611ad-103">لقد اكتشفنا مشكله محتمله في مؤسستك (إذا لم يتم تصحيحها بواسطة شهر أكتوبر 26th 2018) قد تقطع تدفق البريد إلى الوجات المحلية أو الخارجية.</span><span class="sxs-lookup"><span data-stu-id="611ad-103">We've detected a potential issue with your organization that (if not corrected by October 26th, 2018) might break mail flow to your on-premises or external destinations.</span></span> <span data-ttu-id="611ad-104">بمجرد ان يتم الاتصال مسبقا ، لتبسيط أداره نطاق عناوين IP ، سنقوم بدمج نطاقات عناوين IP ل Exchange Online Protection (EOP) التي يتم استخدامها لإرسال البريد الكتروني وتلقيه خارج Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="611ad-104">As previously communicated, to simplify IP address range management, we're consolidating the Exchange Online Protection (EOP) IP address ranges that are used to send and receive email outside of Microsoft 365.</span></span> <span data-ttu-id="611ad-105">يشير التحليل الخاص بنا إلى ان واحد أو أكثر من مصادر البريد الكتروني الخارجية أو الوجات التي قمت بتكوينها في موصلات تدفق البريد لا تقبل الاتصالات من نطاقات عناوين IP التي تظهر [هنا](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="611ad-105">Our analysis indicates that one or more of the external email sources or destinations that you've configured in mail flow connectors aren't accepting connections from the IP address ranges shown [here](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="611ad-106">Act قبل أكتوبر 26th تاكد من ان هذه المصادر والوجات ستقبل الاتصالات بكل [عناوين IP المنشورة](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)والتي تم نشرها.</span><span class="sxs-lookup"><span data-stu-id="611ad-106">Act before October 26th to ensure these sources and destinations will accept connections to and from all [published EOP IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

<span data-ttu-id="611ad-107">للحصول علي مزيد من المعلومات حول هذا التغيير ، يرجى مراجعه نشرات مركز الرسائل [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155)أو [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620)أو [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span><span class="sxs-lookup"><span data-stu-id="611ad-107">For more information about this change, please see Message Center posts [MC146155](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC146155), [MC148620](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC148620), or [MC149274](https://portal.office.com/AdminPortal/home?switchtomodern=true#/MessageCenter?id=MC149274).</span></span>

<span data-ttu-id="611ad-108">**ملاحظه**: إذا قمت مسبقا باستخدام IP أو URL للنشر عبر HTML و XML و RSS لتحديثات نقاط النهاية ، فيجب أيضا الترحيل إلى خدمات الويب الجديدة لاتمته أنواع التحديثات هذه.</span><span class="sxs-lookup"><span data-stu-id="611ad-108">**Note**: If you previously used IP or URL publishing via HTML, XML, and RSS for endpoint updates, you also should migrate to the new web services for automating these types of updates.</span></span> <span data-ttu-id="611ad-109">لمزيد من المعلومات ، راجع [فئات نقاط النهاية ل microsoft 365 وعنوان IP ل microsoft 365 وخدمه ويب URL](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span><span class="sxs-lookup"><span data-stu-id="611ad-109">For more information, see [Microsoft 365 endpoint categories and Microsoft 365 IP Address and URL web service](https://techcommunity.microsoft.com/t5/Office-365-Blog/Announcing-Office-365-endpoint-categories-and-Office-365-IP/ba-p/177638).</span></span>
