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
ms.openlocfilehash: 0e683c8266d425be95e87c590d4cb5d56108721a
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207248"
---
# <a name="data-location"></a><span data-ttu-id="0ded8-102">موقع البيانات</span><span class="sxs-lookup"><span data-stu-id="0ded8-102">Data location</span></span>

<span data-ttu-id="0ded8-103">يمكنك عرض موقع المستاجر 365 Office الخاص بك في مركز الاداره أو عن طريق الاتصال ب Exchange عبر الإنترنت عن طريق PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0ded8-103">You can view the location of your Office 365 tenant in the admin center or by connecting to Exchange Online via PowerShell.</span></span>


<span data-ttu-id="0ded8-104">**مركز الاداره:**</span><span class="sxs-lookup"><span data-stu-id="0ded8-104">**Admin center:**</span></span>
1. <span data-ttu-id="0ded8-105">قم بتسجيل الدخول إلى [مركز الاداره](https://admin.microsoft.com/Adminportal/Home).</span><span class="sxs-lookup"><span data-stu-id="0ded8-105">Log in to the [admin center](https://admin.microsoft.com/Adminportal/Home).</span></span>
2. <span data-ttu-id="0ded8-106">حدد **إعدادات** > **ملف تعريف المؤسسة**.</span><span class="sxs-lookup"><span data-stu-id="0ded8-106">Select **Settings** > **Organization profile**.</span></span>
3. <span data-ttu-id="0ded8-107">ضمن **موقع البيانات**، حدد **عرض التفاصيل**.</span><span class="sxs-lookup"><span data-stu-id="0ded8-107">Under **Data location**, select **View details**.</span></span>


<span data-ttu-id="0ded8-108">**Powershell:**</span><span class="sxs-lookup"><span data-stu-id="0ded8-108">**PowerShell:**</span></span>
1. <span data-ttu-id="0ded8-109">الاتصال ب Exchange عبر الإنترنت باستخدام Windows PowerShell.</span><span class="sxs-lookup"><span data-stu-id="0ded8-109">Connect to Exchange Online by using Windows PowerShell.</span></span>
2. <span data-ttu-id="0ded8-110">تنفيذ cmdlet [الحصول علي اورجانيوناليونيت](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) لعرض قائمه خصائص المستاجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="0ded8-110">Execute the [Get-OrganizationalUnit](https://docs.microsoft.com/en-us/powershell/module/exchange/active-directory/get-organizationalunit) cmdlet to display a list of your tenant’s properties.</span></span> 
3. <span data-ttu-id="0ded8-111">انظر إلى الخاصية اورجانيونيونيد.</span><span class="sxs-lookup"><span data-stu-id="0ded8-111">Look at the OrganizationId property.</span></span>

<span data-ttu-id="0ded8-112">عندما يكون لديك موقع البيانات ل EXO و الاستراتيجي ، يمكنك تحديد موقع البيانات لخدمات أخرى يمكنك [استخدامها من حيث توجد البيانات الخاصة بك](https://products.office.com/where-is-your-data-located).</span><span class="sxs-lookup"><span data-stu-id="0ded8-112">When you have the data location for EXO and SPO, you can determine the data location for other services you may use from [Where your data is located](https://products.office.com/where-is-your-data-located).</span></span>