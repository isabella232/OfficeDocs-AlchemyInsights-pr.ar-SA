---
title: شراء الخدمة الذاتية ل PowerShell
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739957"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="7e1b7-102">شراء الخدمة الذاتية ل PowerShell</span><span class="sxs-lookup"><span data-stu-id="7e1b7-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="7e1b7-103">لاستخدام الوحدة النمطية ل مسكوميرسي PowerShell ، يجب تثبيته علي جهاز Windows 10 باستخدام الأمرين TLS 1.2 (مطلوب أذونات المسؤول المحلي).</span><span class="sxs-lookup"><span data-stu-id="7e1b7-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="7e1b7-104">استيراد الوحدة النمطية مسكوميرسي والاتصال بها.</span><span class="sxs-lookup"><span data-stu-id="7e1b7-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="7e1b7-105">عند المطالبة بتسجيل الدخول ، ستحتاج إلى استخدام بيانات اعتماد دور مسؤول الفوترة أو العمومية.</span><span class="sxs-lookup"><span data-stu-id="7e1b7-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="7e1b7-106">إذا لم يكن لديك TLS 1.2 ، فقد تتلقي رسالة الخطا التالية عند محاولة الحصول علي النهج أو تحديثه:</span><span class="sxs-lookup"><span data-stu-id="7e1b7-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="7e1b7-107">*ارورميساجي-تم إغلاق الاتصال الأساسي: حدث خطا غير متوقع في الإرسال*.</span><span class="sxs-lookup"><span data-stu-id="7e1b7-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



