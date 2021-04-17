---
title: Antispam - 5.7.23
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: e494e8017f24d65a94d1a7490be4d67c46a2120b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821398"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="99dc7-102">إصلاح مشاكل تسليم البريد الإلكتروني لرمز الخطأ 5.7.23</span><span class="sxs-lookup"><span data-stu-id="99dc7-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="99dc7-103">تحقق من سجل SPF DNS لمجالك في مدقق سجلات SPF أو DNS متوفر بشكل عام على الويب.</span><span class="sxs-lookup"><span data-stu-id="99dc7-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="99dc7-104">تحقق من أن الرسالة الصادرة لم يتم تعريفها كرسالة عشوائية من قبل Microsoft، وقد تم توجيهها عبر "تجمع التسليم [عالي المخاطر".](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages)</span><span class="sxs-lookup"><span data-stu-id="99dc7-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="99dc7-105">لن تجتاز الرسائل في "تجمع التسليم عالي المخاطر" عمليات التحقق من SPF، وبالتالي لن تقبلها مؤسسة البريد الإلكتروني الوجهة.</span><span class="sxs-lookup"><span data-stu-id="99dc7-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="99dc7-106">إذا استمرت المشكلة، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الإلكتروني إليه.</span><span class="sxs-lookup"><span data-stu-id="99dc7-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="99dc7-107">دون الخطأ الخارجي المفصل المتوفر في رسالة المرتد.</span><span class="sxs-lookup"><span data-stu-id="99dc7-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="99dc7-108">قد لا يتمكن دعم Microsoft من المساعدة بشكل أكبر.</span><span class="sxs-lookup"><span data-stu-id="99dc7-108">Microsoft support may not be able to assist further.</span></span>
