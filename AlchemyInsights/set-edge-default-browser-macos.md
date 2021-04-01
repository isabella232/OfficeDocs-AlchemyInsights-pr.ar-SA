---
title: تعيين Microsoft Edge كمستعرض افتراضي على جهاز macOS
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491298"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="fc927-102">تعيين Microsoft Edge كمستعرض افتراضي على جهاز macOS</span><span class="sxs-lookup"><span data-stu-id="fc927-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="fc927-103">استخدم أحد هذين الأساليب لتعيين Microsoft Edge كمستعرض افتراضي:</span><span class="sxs-lookup"><span data-stu-id="fc927-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="fc927-104">الطريقة 1: قم بوميض الجهاز بصورة macOS حيث تم تعيين Microsoft Edge بالفعل كمستعرض افتراضي.</span><span class="sxs-lookup"><span data-stu-id="fc927-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="fc927-105">الطريقة 2: تعيين النهج DefaultBrowserSettingEnabled لمطالبة المستخدم بتعيين Microsoft Edge كمستعرض افتراضي.</span><span class="sxs-lookup"><span data-stu-id="fc927-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="fc927-106">يسمح أي من الأسلوبين للمستخدم بتغيير المستعرض الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="fc927-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="fc927-107">لهذا السبب، نوصي بنشر النهج DefaultBrowserSettingEnabled حتى لو استخدمت الأسلوب 1.</span><span class="sxs-lookup"><span data-stu-id="fc927-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="fc927-108">إذا قام مستخدم بتغيير المستعرض الافتراضي بعد نشر النهج، يطالب النهج المستخدم بتعيين المستعرض الافتراضي مرة أخرى إلى Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="fc927-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
