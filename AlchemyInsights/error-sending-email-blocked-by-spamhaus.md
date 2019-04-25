---
title: خطأ في إرسال رسالة بريد إلكتروني يتم حظره بواسطة SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 7d6ad2667613ae948a4abcefafe8d91cf89d2418
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402246"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="7f809-102">خطأ في إرسال البريد الإلكتروني: حظر استخدام Spamhaus المضيف العميل</span><span class="sxs-lookup"><span data-stu-id="7f809-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="7f809-103">عنوان IP الذي يرسل الرسالة موجودة على قائمة حظر المملوكة [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="7f809-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="7f809-104">حسابات المكسور، من بين أسباب منع قبل Spamhaus اختراق أجهزة مشاركة عنوان IP عمومي، ونهج موفر خدمة إنترنت (ISP).</span><span class="sxs-lookup"><span data-stu-id="7f809-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="7f809-105">الإصلاحات الممكنة:</span><span class="sxs-lookup"><span data-stu-id="7f809-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="7f809-106">مع الرسائل الواردة الممنوعة بحيث يمكنك التحكم خادم البريد الإلكتروني مصدر Office 365، تحتاج لتحديد السبب وإزالة الكتلة من موقع Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="7f809-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>
    
- <span data-ttu-id="7f809-107">المحظورة مع الرسائل الواردة إلى Office 365 حيث ينتمي عنوان IP المصدر لشخص آخر مالك عنوان يحتاج إلى إزالة الحظر من موقع Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="7f809-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="7f809-108">إذا كان عنوان IP على قائمة الحظر نهج (PBL)، يمكن تعيين عنوان IP ثابت آخر المالك أو إزالة العنوان من PBL.</span><span class="sxs-lookup"><span data-stu-id="7f809-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>
    
- <span data-ttu-id="7f809-109">الرسائل الصادرة الممنوعة من المجال الخاص بك Office 365، يمكن تلقي هذا الخطأ إذا كان يتم توجيه الرسائل من خلال خدمة طرف ثالث.</span><span class="sxs-lookup"><span data-stu-id="7f809-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="7f809-110">يمكنك استخدام أداة بحث WHOIS للبحث عن مالك عنوان IP المحظورة.</span><span class="sxs-lookup"><span data-stu-id="7f809-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
    

