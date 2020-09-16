---
title: تعذر تعيين نهج اللووسيلفسيرفيسيبوركهاسي أو عرضه
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
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735186"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="fc63c-102">تعذر تعيين نهج اللووسيلفسيرفيسيبوركهاسي أو عرضه</span><span class="sxs-lookup"><span data-stu-id="fc63c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="fc63c-103">عند محاولة تعيين النهج اللووسيلفسيرفيسيبوركهاسي أو عرضه ، تتلقي رسالة الخطا التالية:</span><span class="sxs-lookup"><span data-stu-id="fc63c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="fc63c-104">*هاندليرور: فشل استرداد نهج المنتج باستخدام بوليسييد ' اللووسيلفسيرفيسيبوركهاسي ' ، ارورميساجي-تم إغلاق الاتصال الأساسي: حدث خطا غير متوقع في الإرسال.*</span><span class="sxs-lookup"><span data-stu-id="fc63c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="fc63c-105">قد يعود ذلك إلى إصدار سابق من أمان طبقه النقل (TLS).</span><span class="sxs-lookup"><span data-stu-id="fc63c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="fc63c-106">للاتصال بخدمه مسكوميرسي ، يجب استخدام TLS 1.2 أو الأحدث.</span><span class="sxs-lookup"><span data-stu-id="fc63c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="fc63c-107">جرب الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2 والتحقق منه وأعاده المحاولة.</span><span class="sxs-lookup"><span data-stu-id="fc63c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="fc63c-108">في موجه الأوامر PowerShell (PS C: \) ادخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:</span><span class="sxs-lookup"><span data-stu-id="fc63c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="fc63c-109">تاكد من استخدام الأمر (بروتوكولات) TLS ، وذلك بالأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="fc63c-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="fc63c-110">أعد محاولة تنفيذ الأمرين Get أو Update كما تقتضي الحاجة.</span><span class="sxs-lookup"><span data-stu-id="fc63c-110">Retry the Get or Update commands as needed.</span></span>

