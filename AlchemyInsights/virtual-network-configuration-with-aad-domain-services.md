---
title: التكوين الظاهري مع خدمات مجال AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884803"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="26824-102">التكوين الظاهري مع خدمات مجال AAD</span><span class="sxs-lookup"><span data-stu-id="26824-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="26824-103">يشمل التكوين الافتراضي مع خدمات مجال AAD الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="26824-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="26824-104">التحقق من صحة المجال علي مدخل Azure https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="26824-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="26824-105">التحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة لاجراء المزامنة في خدمات مجال Azure AD علي المدخل https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="26824-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="26824-106">التاكد من ان الشبكة الظاهرية لديك يتم نشرها في نفس منطقه Azure الخاصة بالمجالات المدارة في Azure AD.</span><span class="sxs-lookup"><span data-stu-id="26824-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="26824-107">التاكد من انك لا تملك مجالا موجودا باسم المجال نفسه المتوفر علي الشبكة الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="26824-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="26824-108">للحصول علي مزيد من التفاصيل حول اعتبار التصميم علي الشبكة الظاهرية في Azure لدعم خدمات مجالات AAD ، راجع [اعتبارات الشبكة الظاهرية](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="26824-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

