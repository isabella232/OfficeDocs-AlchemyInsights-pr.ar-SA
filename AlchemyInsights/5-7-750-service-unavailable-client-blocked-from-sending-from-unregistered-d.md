---
title: 1048 5.7.750 خدمه غير متوفرة. حظر العميل من الإرسال من المجالات غير المسجلة
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 731aa2e155ba3fdaaca7fed9dd51b3e4a3f20f29
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664229"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="5d5b9-103">تم حظر عميل 5.7.750 من الإرسال من مجال غير مسجل</span><span class="sxs-lookup"><span data-stu-id="5d5b9-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="5d5b9-104">يحدث الخطا عند إرسال مستوي كبير من الرسائل من المجالات التي لم يتم توفيرها في المستاجر (تمت اضافته كمجالات مقبوله وتم التحقق من صحتها).</span><span class="sxs-lookup"><span data-stu-id="5d5b9-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="5d5b9-105">لتجنب هذا الخطا ، يمكنك استخدام موصل تدفق بريد قائم علي الشهادة حيث يكون مجال الشهادة مجالا موفرا ، أو يمكنك تقديم كل مجالات الإرسال.</span><span class="sxs-lookup"><span data-stu-id="5d5b9-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
