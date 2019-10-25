---
title: مضاد البريد المزعج-5.7.23
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
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682016"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a><span data-ttu-id="5194f-102">إصلاح مشكلات تسليم البريد الكتروني لرمز الخطا 5.7.23</span><span class="sxs-lookup"><span data-stu-id="5194f-102">Fix email delivery issues for error code 5.7.23</span></span>

<span data-ttu-id="5194f-103">تحقق من سجل DNS SPF للمجال الخاص بك في مدقق سجلات SPF أو DNS المتوفرة للعامة علي الويب.</span><span class="sxs-lookup"><span data-stu-id="5194f-103">Verify the SPF DNS record for your domain at a publicly available SPF or DNS record checker on the web.</span></span>

<span data-ttu-id="5194f-104">تحقق من ان الرسالة الصادرة لم يتم تعريفها كرسائل غير مرغوب فيها بواسطة Office 365 وتوجيهها عبر [تجمع التسليم عالي المخاطر](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span><span class="sxs-lookup"><span data-stu-id="5194f-104">Verify that the outbound message wasn't identified as spam by Office 365 and routed through the [High Risk Delivery Pool](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages).</span></span> <span data-ttu-id="5194f-105">الرسائل في تجمع التسليم عاليه المخاطر لن تمر الشيكات SPF ، التالي لن تكون مقبوله من قبل مؤسسه البريد الكتروني الوجهة.</span><span class="sxs-lookup"><span data-stu-id="5194f-105">Messages in the High Risk Delivery Pool won't pass SPF checks, and therefore won't be accepted by the destination email organization.</span></span>

<span data-ttu-id="5194f-106">إذا استمرت المشكلة ، قد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الكتروني.</span><span class="sxs-lookup"><span data-stu-id="5194f-106">If the problem persists, you may need to contact the admin of the mail host to which you are attempting to send email.</span></span> <span data-ttu-id="5194f-107">قم بتدوين الخطا الخارجي المفصل المتوفر في رسالة الارتداد.</span><span class="sxs-lookup"><span data-stu-id="5194f-107">Make note of the detailed external error available in the bounce message.</span></span>  <span data-ttu-id="5194f-108">قد لا يتمكن دعم Office 365 من المساعدة بشكل أكبر.</span><span class="sxs-lookup"><span data-stu-id="5194f-108">Office 365 support may not be able to assist further.</span></span>