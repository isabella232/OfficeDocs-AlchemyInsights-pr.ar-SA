---
title: شراء الخدمة الذاتية من PowerShell
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797708"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="96347-102">شراء الخدمة الذاتية من PowerShell</span><span class="sxs-lookup"><span data-stu-id="96347-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="96347-103">لاستخدام وحدة MSCommerce PowerShell النمطية، تحتاج إلى تثبيتها على جهاز يعمل بنظام التشغيل Windows 10 باستخدام TLS 1.2 (أذونات المسؤول المحلي مطلوبة).</span><span class="sxs-lookup"><span data-stu-id="96347-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="96347-104">استيراد وحدة MSCommerce النمطية والاتصال بها.</span><span class="sxs-lookup"><span data-stu-id="96347-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="96347-105">عند مطالبتك بتسجيل الدخول، ستحتاج إلى استخدام بيانات اعتماد دور مسؤول الفوترة أو العام.</span><span class="sxs-lookup"><span data-stu-id="96347-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="96347-106">إذا لم يكن لديك TLS 1.2، فقد تتلقى الخطأ التالي عند محاولة الحصول على النهج أو تحديثه:</span><span class="sxs-lookup"><span data-stu-id="96347-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="96347-107">*ErrorMessage -تم إغلاق* الاتصال الأساسي: حدث خطأ غير متوقع في عملية إرسال .</span><span class="sxs-lookup"><span data-stu-id="96347-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



