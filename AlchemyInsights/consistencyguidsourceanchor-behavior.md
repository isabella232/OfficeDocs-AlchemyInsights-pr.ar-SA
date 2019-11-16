---
title: السلوك المتناسق/الدليل المرجعي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516951"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="d6d55-102">السلوك المتناسق/الدليل المرجعي</span><span class="sxs-lookup"><span data-stu-id="d6d55-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="d6d55-103">الإعلان Azure الاتصال (الإصدار 1.1.524.0 وبعد) الآن يسهل استخدام السمة الخاصة بالاسم الثابت.</span><span class="sxs-lookup"><span data-stu-id="d6d55-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="d6d55-104">عند استخدام هذه الميزة الاتصال AD Azure تلقائيا بتكوين قواعد المزامنة إلى:</span><span class="sxs-lookup"><span data-stu-id="d6d55-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="d6d55-105">استخدام الخصائص الثابتة كسمه المرجع لكائنات المستخدم.</span><span class="sxs-lookup"><span data-stu-id="d6d55-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="d6d55-106">يتم استخدام ObjectGUID لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="d6d55-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="d6d55-107">بالنسبة لأي كائن المستخدم AD المحلية التي لا يتم تعبئة السمة الخاصة به التي لا يتم نشرها ، Azure AD الاتصال يكتب القيمة objectGUID الخاصة به إلى السمة-المنطقية القوية في "Active Directory" المحلي.</span><span class="sxs-lookup"><span data-stu-id="d6d55-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="d6d55-108">بعد ان يتم تعبئة السمة-التناسق الذي تم ملؤه ، أزور الإعلان الاتصال ثم تصدير الكائن إلى AD Azure.</span><span class="sxs-lookup"><span data-stu-id="d6d55-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="d6d55-109">**ملاحظه:** بمجرد استيراد كائن AD داخلي إلى الاتصال AD Azure (اي ، استيراد إلى مساحة موصل AD والمتوقعة في Metaverse) ، لا يمكنك تغيير قيمه الدليل الخاص به بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="d6d55-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="d6d55-110">لتحديد قيمه المرجع لكائن AD داخلي معين ، قم بتكوين السمة الخاصة به الخاصة بالمسدسات المنطقية قبل استيرادها إلى اتصال AD Azure.</span><span class="sxs-lookup"><span data-stu-id="d6d55-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="d6d55-111">لمزيد من المعلومات حول المرجع والتناسق ، راجع ما يلي: [الاتصال الإعلان Azure: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="d6d55-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

