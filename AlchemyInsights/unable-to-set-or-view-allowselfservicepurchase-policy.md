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
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158541"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="252fa-102">غير قادر على تعيين أو عرض نهج AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="252fa-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="252fa-103">عند محاولة تعيين أو عرض نهج AllowSelfServicePurchase، تتلقى رسالة الخطأ التالية:</span><span class="sxs-lookup"><span data-stu-id="252fa-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="252fa-104">*مؤشر الخطأ: فشل في استرداد نهج المنتج باستخدام PolicyId "AllowSelfServicePurchase"، خطأرسالة - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال.*</span><span class="sxs-lookup"><span data-stu-id="252fa-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="252fa-105">قد يكون هذا بسبب إصدار أقدم من أمان طبقة النقل (TLS).</span><span class="sxs-lookup"><span data-stu-id="252fa-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="252fa-106">لتوصيل خدمة MSCommerce ، تحتاج إلى استخدام TLS 1.2 أو أكبر.</span><span class="sxs-lookup"><span data-stu-id="252fa-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="252fa-107">حاول الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2، تحقق، وإعادة المحاولة.</span><span class="sxs-lookup"><span data-stu-id="252fa-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="252fa-108">في موجه الأمر PowerShell (PS C:\) أدخل الأمر التالي لتعيين بروتوكول TLS إلى الإصدار 1.2:</span><span class="sxs-lookup"><span data-stu-id="252fa-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="252fa-109">تحقق من بروتوكول TLS (البروتوكولات) في الاستخدام، مع الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="252fa-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="252fa-110">إعادة محاولة أوامر الحصول على أو تحديث حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="252fa-110">Retry the Get or Update commands as needed.</span></span>

