---
title: أنتيسبام-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717312"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="ae0ab-102">إصلاح مشاكل تسليم البريد الكتروني لرمز الخطا 5.7.23</span><span class="sxs-lookup"><span data-stu-id="ae0ab-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="ae0ab-103">تاكد من ان سجل DNS SPF لمجالك لديك بشكل عام SPF أو مدقق سجلات DNS علي الويب.</span><span class="sxs-lookup"><span data-stu-id="ae0ab-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="ae0ab-104">تاكد من ان الرسالة الصادرة لم يتم تحديدها كبريد عشوائي بواسطة Microsoft وموجهه عبر [تجمع التسليم عالي الجودة](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="ae0ab-104">Verify that the outbound message wasn't identified as spam by Microsoft and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="ae0ab-105">لن تنجح الرسائل الموجودة في تجمع التسليم عالي المخاطرة في إيداع SPF ، التالي لن يتم قبولها بواسطة مؤسسه البريد الكتروني الوجهة.</span><span class="sxs-lookup"><span data-stu-id="ae0ab-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="ae0ab-106">إذا استمرت المشكلة ، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الكتروني اليه.</span><span class="sxs-lookup"><span data-stu-id="ae0ab-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="ae0ab-107">قم بتدوين الخطا الخارجي المفصل المتوفر في رسالة وثبات.</span><span class="sxs-lookup"><span data-stu-id="ae0ab-107">Make note of the detailed external error available in the bounce message.</span></span> <span data-ttu-id="ae0ab-108">قد لا يتمكن دعم Microsoft من المساعدة.</span><span class="sxs-lookup"><span data-stu-id="ae0ab-108">Microsoft support may not be able to assist further.</span></span>
