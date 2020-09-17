---
title: خطا في إرسال البريد الكتروني المحظور بواسطة SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783754"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="3f0dc-102">خطا في إرسال البريد الكتروني: تم حظر مضيف العميل باستخدام Spamhaus</span><span class="sxs-lookup"><span data-stu-id="3f0dc-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="3f0dc-103">يكون عنوان IP الذي أرسل الرسالة في قائمه حظر مملوكه ل [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="3f0dc-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="3f0dc-104">تشمل الأسباب التي يتم حظرها بواسطة Spamhaus الحسابات التي تم اختراقها ومشاركه عناوين IP العامة ونهج موفر خدمه الإنترنت (ISP).</span><span class="sxs-lookup"><span data-stu-id="3f0dc-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="3f0dc-105">التصحيحات المحتملة هي:</span><span class="sxs-lookup"><span data-stu-id="3f0dc-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="3f0dc-106">بالنسبة إلى الرسائل الواردة المحظورة حيث تتحكم في خادم البريد الكتروني المصدر ، يجب تحديد السبب وأزاله الحظر من موقع Spamhaus علي ويب.</span><span class="sxs-lookup"><span data-stu-id="3f0dc-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="3f0dc-107">بالنسبة إلى الرسائل الواردة المحظورة التي ينتمي اليها عنوان IP المصدر لشخص آخر ، يحتاج مالك العنوان إلى أزاله الحظر من موقع ويب Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="3f0dc-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="3f0dc-108">إذا كان عنوان IP في قائمه حظر النهج (ببل) ، فبامكان المالك تعيين عنوان IP ثابت مختلف أو أزاله العنوان من ببل.</span><span class="sxs-lookup"><span data-stu-id="3f0dc-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="3f0dc-109">بالنسبة إلى الرسائل الصادرة المحظورة من المجال المتصل ب Microsoft ، يمكنك تلقي هذا الخطا إذا كانت الرسائل موجهه عبر خدمه الطرف الخارجي.</span><span class="sxs-lookup"><span data-stu-id="3f0dc-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="3f0dc-110">يمكنك استخدام أداه البحث في WHOIS للعثور علي مالك عنوان IP المحظور.</span><span class="sxs-lookup"><span data-stu-id="3f0dc-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
