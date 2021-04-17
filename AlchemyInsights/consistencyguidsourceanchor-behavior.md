---
title: سلوك التناسقGuid / sourceAnchor
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816979"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="81983-102">سلوك التناسقGuid / sourceAnchor</span><span class="sxs-lookup"><span data-stu-id="81983-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="81983-103">يسهل Azure AD Connect (الإصدار 1.1.524.0 وما بعده) الآن استخدام msDS-ConsistencyGuid ك سمة sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="81983-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="81983-104">عند استخدام هذه الميزة، يقوم Azure AD Connect تلقائيا بتكوين قواعد المزامنة من أجل:</span><span class="sxs-lookup"><span data-stu-id="81983-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="81983-105">استخدم msDS-ConsistencyGuid ك السمة sourceAnchor كائنات المستخدم.</span><span class="sxs-lookup"><span data-stu-id="81983-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="81983-106">يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="81983-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="81983-107">بالنسبة لأي كائن مستخدم AD موقعي معين لم يتم ملء سمة msDS-ConsistencyGuid الخاصة به، يقوم Azure AD Connect بكتابة قيمة كائنGUID الخاصة به مرة أخرى إلى السمة msDS-ConsistencyGuid في Active Directory في الموقع.</span><span class="sxs-lookup"><span data-stu-id="81983-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="81983-108">بعد تعبئة السمة msDS-ConsistencyGuid، يصدر Azure AD Connect الكائن إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="81983-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="81983-109">**ملاحظة:** بمجرد استيراد كائن AD المحلي إلى Azure AD Connect (أي، استيراده إلى "مساحة موصل AD" والتوقع إلى Metaverse)، لا يمكنك تغيير قيمة sourceAnchor الخاصة به بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="81983-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="81983-110">لتحديد قيمة sourceAnchor لكائن AD معين في الموقع، قم بتكوين السمة msDS-ConsistencyGuid قبل استيرادها إلى Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="81983-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="81983-111">لمزيد من المعلومات حول SourceAnchor وتناسقGuid، راجع ما [يلي: Azure AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="81983-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

