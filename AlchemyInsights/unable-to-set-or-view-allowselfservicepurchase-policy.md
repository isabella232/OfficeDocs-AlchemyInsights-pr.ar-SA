---
title: غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: a9b6e36e8034e71b3e72c49e3cc68a126ef97aca
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091654"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="12e8c-102">غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="12e8c-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="12e8c-103">عند محاولة تعيين أو عرض نهج AllowSelfServicePurchase، تتلقى رسالة الخطأ التالية:</span><span class="sxs-lookup"><span data-stu-id="12e8c-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="12e8c-104">*مؤشر الخطأ: فشل في استرداد نهج المنتج باستخدام PolicyId "AllowSelfServicePurchase"، خطأرسالة - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال.*</span><span class="sxs-lookup"><span data-stu-id="12e8c-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="12e8c-105">قد يكون هذا بسبب إصدار أقدم من أمان طبقة النقل (TLS).</span><span class="sxs-lookup"><span data-stu-id="12e8c-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="12e8c-106">لتوصيل خدمة MSCommerce ، تحتاج إلى استخدام TLS 1.2 أو أكبر.</span><span class="sxs-lookup"><span data-stu-id="12e8c-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="12e8c-107">حاول الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2، تحقق، وإعادة المحاولة.</span><span class="sxs-lookup"><span data-stu-id="12e8c-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="12e8c-108">في موجه الأمر PowerShell (PS C:\) أدخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:</span><span class="sxs-lookup"><span data-stu-id="12e8c-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    <span data-ttu-id="12e8c-109">\[Net.ServicePointManager]::بروتوكول الأمن \[= Net.SecurityProtocolType]::Tls12</span><span class="sxs-lookup"><span data-stu-id="12e8c-109">\[Net.ServicePointManager]::SecurityProtocol = \[Net.SecurityProtocolType]::Tls12</span></span>

2. <span data-ttu-id="12e8c-110">تحقق من بروتوكول TLS (البروتوكولات) في الاستخدام، مع الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="12e8c-110">Verify the TLS protocol(s) in use, with the following command:</span></span>

    <span data-ttu-id="12e8c-111">\[Net.ServicePointManager]::بروتوكول الأمن</span><span class="sxs-lookup"><span data-stu-id="12e8c-111">\[Net.ServicePointManager]::SecurityProtocol</span></span> 

3. <span data-ttu-id="12e8c-112">إعادة محاولة أوامر الحصول على أو تحديث حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="12e8c-112">Retry the Get or Update commands as needed.</span></span>

