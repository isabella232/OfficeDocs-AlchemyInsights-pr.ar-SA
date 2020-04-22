---
title: مكافحة البريد المزعج - 5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 307b738c40c620d057e68eff7d218c8c9b5eb665
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676484"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="48781-102">إصلاح مشكلات تسليم البريد الإلكتروني لرمز الخطأ 5.7.23</span><span class="sxs-lookup"><span data-stu-id="48781-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="48781-103">تحقق من سجل DNS SPF للمجال الخاص بك في مدقق سجل SPF أو DNS متوفر بشكل عام على الويب.</span><span class="sxs-lookup"><span data-stu-id="48781-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="48781-104">تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسائل غير مرغوب فيها من قبل Microsoft وتم توجيهها من خلال [تجمع التسليم عالي الخطورة](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="48781-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="48781-105">لن تجتاز الرسائل الموجودة في تجمع التسليم عالي المخاطر شيكات SPF، وبالتالي لن يتم قبولها من قبل مؤسسة البريد الإلكتروني الوجهة.</span><span class="sxs-lookup"><span data-stu-id="48781-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="48781-106">إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال بريد إلكتروني إليه.</span><span class="sxs-lookup"><span data-stu-id="48781-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="48781-107">دوّن الخطأ الخارجي المفصل المتوفر في رسالة الارتداد.</span><span class="sxs-lookup"><span data-stu-id="48781-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="48781-108">قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.</span><span class="sxs-lookup"><span data-stu-id="48781-108">Microsoft support may not be able to assist further.</span></span>
