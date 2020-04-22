---
title: خطأ في إرسال البريد الإلكتروني المحظور من قبل SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714245"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="ee370-102">خطأ إرسال البريد الإلكتروني: تم حظر مضيف العميل باستخدام Spamhaus</span><span class="sxs-lookup"><span data-stu-id="ee370-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="ee370-103">عنوان IP الذي أرسل الرسالة موجود على قائمة حظر مملوكة من [قبل Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="ee370-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="ee370-104">تتضمن أسباب حظرالبريد الإلكتروني غير المرغوب فيه الحسابات التي تم اختراقها، والآلات التي تم اختراقها التي تشارك عنوان IP عامًا، وسياسات موفر خدمة الإنترنت (ISP).</span><span class="sxs-lookup"><span data-stu-id="ee370-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="ee370-105">الإصلاحات المحتملة هي:</span><span class="sxs-lookup"><span data-stu-id="ee370-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="ee370-106">بالنسبة للرسائل الواردة المحظورة حيث تتحكم في خادم البريد الإلكتروني المصدر، تحتاج إلى تحديد السبب وإزالة الحظر من موقع Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ee370-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="ee370-107">بالنسبة للرسائل الواردة المحظورة حيث ينتمي عنوان IP المصدر إلى شخص آخر ، يحتاج مالك العنوان إلى إزالة الحظر من موقع Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="ee370-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="ee370-108">إذا كان عنوان IP موجودًا في قائمة كتلة النهج (PBL)، يمكن للمالك تعيين عنوان IP ثابت مختلف أو إزالة العنوان من PBL.</span><span class="sxs-lookup"><span data-stu-id="ee370-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="ee370-109">بالنسبة للرسائل الصادرة المحظورة من نطاقك المتصل بـ Microsoft، يمكنك تلقي هذا الخطأ إذا تم توجيه الرسائل من خلال خدمة جهة خارجية.</span><span class="sxs-lookup"><span data-stu-id="ee370-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="ee370-110">يمكنك استخدام أداة بحث WHOIS للعثور على مالك عنوان IP المحظور.</span><span class="sxs-lookup"><span data-stu-id="ee370-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
