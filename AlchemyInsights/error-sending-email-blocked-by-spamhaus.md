---
title: خطأ في إرسال بريد إلكتروني تم حظره بواسطة SpamHaus
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813711"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="eff8c-102">خطأ في إرسال البريد الإلكتروني: تم حظر مضيف العميل باستخدام Spamhaus</span><span class="sxs-lookup"><span data-stu-id="eff8c-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="eff8c-103">يوجد عنوان IP الذي أرسل الرسالة في قائمة الحظر التي يملكها [Spamhaus.](https://go.microsoft.com/fwlink/p/?linkid=123245)</span><span class="sxs-lookup"><span data-stu-id="eff8c-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="eff8c-104">تتضمن أسباب حظر البريد العشوائي الحسابات الم اختراق الأجهزة التي تشارك عنوان IP عام ونهج موفر خدمة الإنترنت (ISP).</span><span class="sxs-lookup"><span data-stu-id="eff8c-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="eff8c-105">الإصلاحات المحتملة هي:</span><span class="sxs-lookup"><span data-stu-id="eff8c-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="eff8c-106">بالنسبة للرسائل الواردة المحظورة حيث تتحكم في خادم البريد الإلكتروني المصدر، ستحتاج إلى تحديد السبب وإزالة الحظر من موقع Spamhaus على الويب.</span><span class="sxs-lookup"><span data-stu-id="eff8c-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="eff8c-107">بالنسبة للرسائل الواردة المحظورة التي ينتمي فيها عنوان IP المصدر إلى شخص آخر، يحتاج مالك العنوان إلى إزالة الحظر من موقع Spamhaus على الويب.</span><span class="sxs-lookup"><span data-stu-id="eff8c-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="eff8c-108">إذا كان عنوان IP في قائمة حظر النهج (PBL)، يمكن للمالك تعيين عنوان IP ثابت مختلف أو إزالة العنوان من PBL.</span><span class="sxs-lookup"><span data-stu-id="eff8c-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="eff8c-109">بالنسبة للرسائل الصادرة المحظورة من مجالك المتصل ب Microsoft، يمكنك تلقي هذا الخطأ إذا تم توجيه الرسائل عبر خدمة جهة خارجية.</span><span class="sxs-lookup"><span data-stu-id="eff8c-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="eff8c-110">يمكنك استخدام أداة البحث WHOIS للعثور على مالك عنوان IP المحظور.</span><span class="sxs-lookup"><span data-stu-id="eff8c-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
