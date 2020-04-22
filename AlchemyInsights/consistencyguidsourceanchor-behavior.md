---
title: ConsistencyGuid / سلوك مرساة المصدر
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705720"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="aeaf4-102">ConsistencyGuid / سلوك مرساة المصدر</span><span class="sxs-lookup"><span data-stu-id="aeaf4-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="aeaf4-103">Azure AD Connect (الإصدار 1.1.524.0 وما بعده) يسهل الآن استخدام msDS-ConsistencyGuid كسمة sourceAnchor.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="aeaf4-104">عند استخدام هذه الميزة، يقوم Azure AD Connect بتكوين قواعد المزامنة تلقائيًا إلى:</span><span class="sxs-lookup"><span data-stu-id="aeaf4-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="aeaf4-105">استخدم msDS-ConsistencyGuid كسمة sourceAnchor لكائنات المستخدم.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="aeaf4-106">يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="aeaf4-107">لأي كائن مستخدم AD معين داخليًا لا يتم ملء سمة msDS-ConsistencyGuid الخاصة به، يقوم Azure AD Connect بكتابة قيمة objectGUID الخاصة به مرة أخرى إلى سمة msDS-ConsistencyGuid في الدليل النشط الداخلي.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="aeaf4-108">بعد ملء السمة msDS-ConsistencyGuid، يقوم Azure AD Connect بعد ذلك بتصدير الكائن إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="aeaf4-109">**ملاحظة:** بمجرد استيراد كائن AD داخلي إلى Azure AD Connect (أي استيراده إلى مساحة موصل الإعلانية والمتوقع في Metaverse)، لا يمكنك تغيير قيمة المصدر Anchor بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="aeaf4-110">لتحديد قيمة sourceAnchor لكائن AD داخلي معين، قم بتكوين سمة msDS-ConsistencyGuid قبل استيرادها إلى Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="aeaf4-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="aeaf4-111">لمزيد من المعلومات حول SourceAnchor وConsistencyGuid، راجع ما يلي: [Azure AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="aeaf4-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

