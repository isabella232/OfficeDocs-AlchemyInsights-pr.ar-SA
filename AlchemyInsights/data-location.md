---
title: موقع البيانات
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "945"
- "5300023"
ms.assetid: 3bab036c-dbaa-406a-8b73-1e5f31993436
ms.openlocfilehash: c769c17796d805f88afb4d5b32adb7d4a9bb3ce0
ms.sourcegitcommit: 6bf1d945b4fd6a1fe37d00c5ea99adea7eef9910
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/21/2020
ms.locfileid: "43655269"
---
# <a name="data-location"></a><span data-ttu-id="a6d06-102">موقع البيانات</span><span class="sxs-lookup"><span data-stu-id="a6d06-102">Data location</span></span>

<span data-ttu-id="a6d06-103">يمكنك عرض موقع المستأجر الخاص بك في مركز المشرف أو عن طريق الاتصال بExchange Online عبر PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a6d06-103">You can view the location of your tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="a6d06-104">**مركز المشرف:**</span><span class="sxs-lookup"><span data-stu-id="a6d06-104">**Admin center:**</span></span>
1. <span data-ttu-id="a6d06-105">تسجيل الدخول إلى [مركز المشرف](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="a6d06-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="a6d06-106">حدد**ملف تعريف مؤسسة** **الإعدادات** > .</span><span class="sxs-lookup"><span data-stu-id="a6d06-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="a6d06-107">ضمن **موقع البيانات،** حدد **عرض التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="a6d06-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="a6d06-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="a6d06-108">**PowerShell:**</span></span>
1. <span data-ttu-id="a6d06-109">الاتصال بالتبادل عبر الإنترنت باستخدام Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a6d06-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="a6d06-110">تنفيذ [cmdlet الحصول على التنظيمية](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) لعرض قائمة خصائص المستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a6d06-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant's properties.</span></span> 
3. <span data-ttu-id="a6d06-111">انظر إلى خاصية OrganizationId.</span><span class="sxs-lookup"><span data-stu-id="a6d06-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="a6d06-112">عندما يكون لديك موقع البيانات لEXO و SPO، يمكنك تحديد موقع البيانات للخدمات الأخرى التي قد تستخدمها من [حيث توجد البيانات الخاصة بك](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="a6d06-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>