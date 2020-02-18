---
title: شراء الخدمة الذاتية من PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091653"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="50338-102">شراء الخدمة الذاتية من PowerShell</span><span class="sxs-lookup"><span data-stu-id="50338-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="50338-103">لاستخدام وحدة MSCommerce PowerShell، تحتاج إلى تثبيتها على جهاز Windows 10 مع TLS 1.2 (أذونات المسؤول المحلي المطلوبة).</span><span class="sxs-lookup"><span data-stu-id="50338-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="50338-104">استيراد وحدة MSCommerce والاتصال بها.</span><span class="sxs-lookup"><span data-stu-id="50338-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="50338-105">عند المطالبة بتسجيل الدخول، ستحتاج إلى استخدام بيانات اعتماد دور مسؤول الفوترة أو العمومية.</span><span class="sxs-lookup"><span data-stu-id="50338-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="50338-106">إذا لم يكن لديك TLS 1.2، قد تتلقى الخطأ التالي عند محاولة الحصول على النهج أو تحديثه:</span><span class="sxs-lookup"><span data-stu-id="50338-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="50338-107">*خطأرسالة -تم إغلاق الاتصال الأساسي: حدث خطأ غير متوقع على إرسال*.</span><span class="sxs-lookup"><span data-stu-id="50338-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



