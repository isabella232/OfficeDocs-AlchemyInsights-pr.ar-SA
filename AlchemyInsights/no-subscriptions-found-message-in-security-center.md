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
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713266"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="10395-102">لم يتم العثور على أي رسالة اشتراكات في مركز الأمان</span><span class="sxs-lookup"><span data-stu-id="10395-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="10395-103">إذا حصلت على رسالة "لم يتم العثور على اشتراكات" أثناء الوصول إلى مركز أمان Microsoft Defender، فهذا يعني أن Azure Active Directory (AAD) المستخدم لتسجيل دخول المستخدم إلى المدخل ليس لديه ترخيص MICROSOFT Defender ATP.</span><span class="sxs-lookup"><span data-stu-id="10395-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="10395-104">إن تراخيص Windows E5 و Office E5 هي تراخيص منفصلة.</span><span class="sxs-lookup"><span data-stu-id="10395-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="10395-105">افتح حالة دعم إذا تم شراء الترخيص ولكن لم يتم توفيره لمثيل AAD هذا.</span><span class="sxs-lookup"><span data-stu-id="10395-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="10395-106">إما أن يكون لديك:</span><span class="sxs-lookup"><span data-stu-id="10395-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="10395-107">مشكلة محتملة في توفير التراخيص.</span><span class="sxs-lookup"><span data-stu-id="10395-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="10395-108">لقد قمت عن غير قصد بتوفير الترخيص ل Microsoft AAD مختلف عن ذلك المستخدم للمصادقة في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="10395-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>