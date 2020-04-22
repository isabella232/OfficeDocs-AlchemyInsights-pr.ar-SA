---
title: 1048 5.7.750 خدمة غير متوفرة. تم حظر العميل من الإرسال من المجالات غير المسجلة
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676700"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a><span data-ttu-id="c5a39-103">5.7.750 عميل محظور من الإرسال من المجال غير المسجل</span><span class="sxs-lookup"><span data-stu-id="c5a39-103">5.7.750 Client blocked from sending from unregistered domain</span></span>

<span data-ttu-id="c5a39-104">يحدث الخطأ عند إرسال كمية كبيرة من الرسائل من المجالات التي لم يتم توفيرها في المستأجر الخاص بك (تمت إضافتها كمجالات مقبولة والتحقق من صحتها).</span><span class="sxs-lookup"><span data-stu-id="c5a39-104">The error occurs when a large volume of messages are sent from domains that aren't provisioned in your tenant (added as accepted domains and validated).</span></span>

<span data-ttu-id="c5a39-105">لتجنب هذا الخطأ، يمكنك استخدام موصل تدفق بريد يستند إلى الشهادة حيث مجال الشهادة هو مجال تم توفيره، أو يمكنك توفير كافة مجالات الإرسال.</span><span class="sxs-lookup"><span data-stu-id="c5a39-105">To avoid this error, you can use a certificate-based mail flow connector where the certificate's domain is a provisioned domain, or you can provision all sending domains.</span></span>
