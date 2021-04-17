---
title: تعذر تعيين نهج AllowSelfServicePurchase أو عرضه
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
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826078"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="1050d-102">تعذر تعيين نهج AllowSelfServicePurchase أو عرضه</span><span class="sxs-lookup"><span data-stu-id="1050d-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="1050d-103">عند محاولة تعيين نهج AllowSelfServicePurchase أو عرضه، ستتلقى رسالة الخطأ التالية:</span><span class="sxs-lookup"><span data-stu-id="1050d-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="1050d-104">*معالج : فشل استرداد نهج المنتج باستخدام PolicyId 'AllowSelfServicePurchase', ErrorMessage - تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع في عملية إرسال.*</span><span class="sxs-lookup"><span data-stu-id="1050d-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="1050d-105">قد يعود سبب ذلك إلى إصدار أقدم من "أمان طبقة النقل" (TLS).</span><span class="sxs-lookup"><span data-stu-id="1050d-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="1050d-106">لتوصيل خدمة MSCommerce، تحتاج إلى استخدام TLS 1.2 أو أكبر.</span><span class="sxs-lookup"><span data-stu-id="1050d-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="1050d-107">جرب الخطوات التالية لتمكين/تعيين بروتوكول TLS إلى 1.2 والتحقق من الصحة والمحاولة مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="1050d-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="1050d-108">في موجه الأوامر PowerShell (PS C: أدخل الأمر التالي لتعيين \) بروتوكول TLS إلى الإصدار 1.2:</span><span class="sxs-lookup"><span data-stu-id="1050d-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="1050d-109">تحقق من بروتوكول (بروتوكولات) TLS (بروتوكولات) TLS المستخدم، باستخدام الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="1050d-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="1050d-110">إعادة محاولة الأمرين الحصول أو التحديث حسب الحاجة.</span><span class="sxs-lookup"><span data-stu-id="1050d-110">Retry the Get or Update commands as needed.</span></span>

