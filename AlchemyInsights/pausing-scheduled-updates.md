---
title: إيقاف مؤقت للتحديثات المجدولة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/30/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1129"
- "6700007"
ms.openlocfilehash: 13abc7c9201b1897a9c766add4d105ef12f0d66f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47721542"
---
# <a name="pausing-scheduled-updates"></a><span data-ttu-id="ad44d-102">إيقاف مؤقت للتحديثات المجدولة</span><span class="sxs-lookup"><span data-stu-id="ad44d-102">Pausing scheduled updates</span></span>

<span data-ttu-id="ad44d-103">عند إصدار الأمر pause ، لا تعالج الاجهزه الأمر حتى المرة التالية التي يقومون فيها بالإيداع في Intune.</span><span class="sxs-lookup"><span data-stu-id="ad44d-103">When a pause command is issued, devices don't process the command until the next time they check in to Intune.</span></span> <span data-ttu-id="ad44d-104">بسبب هذا ، قد يكون لديك الاجهزه:</span><span class="sxs-lookup"><span data-stu-id="ad44d-104">Because of this, your devices might have:</span></span>

- <span data-ttu-id="ad44d-105">تثبيت التحديثات المجدولة قبل الإيداع.</span><span class="sxs-lookup"><span data-stu-id="ad44d-105">Installed the scheduled updates prior to check-in.</span></span>
- <span data-ttu-id="ad44d-106">تم إيقاف تشغيله عند إصدار الأمر pause.</span><span class="sxs-lookup"><span data-stu-id="ad44d-106">Been powered off when you issued the pause command.</span></span> <span data-ttu-id="ad44d-107">في هذه الحالة ، عندما تكون الاجهزه مشغله ، قد قمت بتنزيل التحديثات المجدولة وتثبيتها قبل الإيداع.</span><span class="sxs-lookup"><span data-stu-id="ad44d-107">In this case, when the devices were powered on, they might have downloaded and installed the scheduled updates prior to check-in.</span></span>