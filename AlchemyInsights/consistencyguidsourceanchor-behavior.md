---
title: سلوك كونسيستينسيجويد/سورسيانتشور
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756270"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="31d70-102">سلوك كونسيستينسيجويد/سورسينتشور</span><span class="sxs-lookup"><span data-stu-id="31d70-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="31d70-103">يسهل الآن Azure AD Connect (الإصدار 1.1.524.0 وما يليه) استخدام السمة مسدس-كونسيستينسيجويد كسورسينتشور.</span><span class="sxs-lookup"><span data-stu-id="31d70-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="31d70-104">عند استخدام هذه الميزة ، يقوم Azure AD بتكوين قواعد المزامنة تلقائيا إلى:</span><span class="sxs-lookup"><span data-stu-id="31d70-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="31d70-105">استخدم مسدس-كونسيستينسيجويد كسمه سورسينتشور لكائنات المستخدم.</span><span class="sxs-lookup"><span data-stu-id="31d70-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="31d70-106">يتم استخدام أوبجيكتجويد لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="31d70-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="31d70-107">بالنسبة إلى اي كائن المستخدم المحلي الخاص بالإعلانات المحددة التي لا يتم تعبئة السمة مسدس الخاصة بها ، فان Azure AD Connect تكتب قيمه أوبجيكتجويد الخاصة بها مره أخرى إلى السمة مسدس-كونسيستينسيجويد في Active Directory المحلي.</span><span class="sxs-lookup"><span data-stu-id="31d70-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="31d70-108">بعد تعبئة السمة مسدس-كونسيستينسيجويد ، يقوم Azure AD Connect بتصدير الكائن إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="31d70-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="31d70-109">**ملاحظه:** بمجرد استيراد كائن الإعلانات المحلي إلى Azure AD Connect (والذي يتم استيراده إلى مساحة موصل الإعلانات وعرضه في ميتافيرسي) ، لا يمكنك تغيير قيمه سورسيانتشور الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="31d70-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="31d70-110">لتحديد القيمة سورسيانتشور لكائن إعلانات معين في الموقع المحلي ، قم بتكوين سمه مسدس-كونسيستينسيجويد قبل استيرادها إلى Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="31d70-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="31d70-111">للحصول علي مزيد من المعلومات حول سورسينتشور و كونسيستينسيجويد ، يمكنك الرجوع إلى ما يلي: [AZURE AD Connect: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="31d70-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

