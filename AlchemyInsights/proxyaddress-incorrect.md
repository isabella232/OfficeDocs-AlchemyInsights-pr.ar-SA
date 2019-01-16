---
title: ProxyAddress غير صحيحة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: 0d7282473822a7c6bad06a1c1d93dbd6f391404b
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273463"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="250f6-102">ProxyAddress غير صحيحة</span><span class="sxs-lookup"><span data-stu-id="250f6-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="250f6-p101">عند مزامنة كائن لإعلان أزور، تتم مقارنة القيم التي تم تعيينها في سمة proxyAddresses في "Active Directory" بقواعد مكافحة الإغراق Azure وثم تعبئة السمة proxyAddresses في الإعلان Azure. وبالتالي، قيم السمة proxyAddresses للكائن في "Active Directory" قد لا نفس قيم السمة proxyAddresses في الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="250f6-p101">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD. Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="250f6-105">لمزيد من المعلومات حول كيف يتم ملؤها proxyaddress، راجع [كيفية تعبئة السمة proxyAddress في الإعلان Azure](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="250f6-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/en-us/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

