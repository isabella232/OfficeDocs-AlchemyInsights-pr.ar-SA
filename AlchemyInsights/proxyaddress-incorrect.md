---
title: ProxyAddress غير صحيحة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: c4cea778-1b26-4aea-bde8-4b7605e35886
ms.openlocfilehash: 1f908b6fca813ff6cbc4d05d08ee2eb9c49f3515
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36554211"
---
# <a name="proxyaddress-incorrect"></a><span data-ttu-id="b9e79-102">ProxyAddress غير صحيحة</span><span class="sxs-lookup"><span data-stu-id="b9e79-102">ProxyAddress incorrect</span></span>

<span data-ttu-id="b9e79-103">عند مزامنة كائن لإعلان أزور، تتم مقارنة القيم التي تم تعيينها في سمة proxyAddresses في "Active Directory" بقواعد مكافحة الإغراق Azure وثم تعبئة السمة proxyAddresses في الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="b9e79-103">When an object is synchronized to Azure AD, the values that are specified in the proxyAddresses attribute in Active Directory are compared with Azure AD rules, and then the proxyAddresses attribute is populated in Azure AD.</span></span> <span data-ttu-id="b9e79-104">وبالتالي، قيم السمة proxyAddresses للكائن في "Active Directory" قد لا نفس قيم السمة proxyAddresses في الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="b9e79-104">Therefore, the values of the proxyAddresses attribute for the object in Active Directory may not be the same as the values of the proxyAddresses attribute in Azure AD.</span></span>
  
<span data-ttu-id="b9e79-105">لمزيد من المعلومات حول كيف يتم ملؤها proxyaddress، راجع [كيفية تعبئة السمة proxyAddress في الإعلان Azure](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span><span class="sxs-lookup"><span data-stu-id="b9e79-105">To learn more about how the proxyaddress is populated, see [How the proxyAddress attribute is populated in Azure AD](https://support.microsoft.com/help/3190357/how-the-proxyaddresses-attribute-is-populated-in-azure-ad).</span></span>
  

