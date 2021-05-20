---
title: لم يتم العثور على أي رسالة اشتراكات في مركز الأمان
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 777fb9b09aa26d166f9971589bda464ccb90f4be
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544095"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bd013-102">لم يتم العثور على أي رسالة اشتراكات في مركز الأمان</span><span class="sxs-lookup"><span data-stu-id="bd013-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bd013-103">إذا لم مركز حماية Microsoft Defender الرسالة "لم يتم العثور على اشتراكات"، فهذا يعني أن Azure Active Directory (AAD) المستخدم لتسجيل دخول المستخدم إلى المدخل لا Microsoft Defender ATP ترخيص.</span><span class="sxs-lookup"><span data-stu-id="bd013-103">If while accessing Microsoft Defender Security Center you get a "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bd013-104">إن Windows E5 Office E5 هي تراخيص منفصلة.</span><span class="sxs-lookup"><span data-stu-id="bd013-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bd013-105">افتح حالة دعم إذا تم شراء الترخيص ولكن لم يتم توفيره لمثيل AAD هذا.</span><span class="sxs-lookup"><span data-stu-id="bd013-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bd013-106">إما أن يكون لديك:</span><span class="sxs-lookup"><span data-stu-id="bd013-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bd013-107">مشكلة محتملة في توفير الترخيص.</span><span class="sxs-lookup"><span data-stu-id="bd013-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bd013-108">لقد قمت عن غير قصد بتوفير الترخيص ل Microsoft AAD مختلف عن ذلك المستخدم للمصادقة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="bd013-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>