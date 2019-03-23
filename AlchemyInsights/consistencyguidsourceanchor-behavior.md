---
title: كونسيستينسيجويد/سورسينتشور السلوك
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
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753089"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="3b77d-102">كونسيستينسيجويد/سورسيانتشور السلوك</span><span class="sxs-lookup"><span data-stu-id="3b77d-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="3b77d-103">الاتصال الإعلان أزور (الإصدار 1.1.524.0 وبعد) يسهل استخدام مسدس كونسيستينسيجويد كسمة سورسينتشور الآن.</span><span class="sxs-lookup"><span data-stu-id="3b77d-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="3b77d-104">عند استخدام هذه الميزة، Azure الإعلان الاتصال تلقائياً بتكوين قواعد المزامنة إلى:</span><span class="sxs-lookup"><span data-stu-id="3b77d-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="3b77d-105">استخدام مسدس كونسيستينسيجويد كسمة سورسينتشور لكائنات المستخدم.</span><span class="sxs-lookup"><span data-stu-id="3b77d-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="3b77d-106">يتم استخدام دليل الكائن لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="3b77d-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="3b77d-107">لأي إعطاء الداخلي المستخدم الإعلان الكائن الذي سمته مسدس كونسيستينسيجويد لا يكتب الاتصال الإعلان المعممة، Azure قيمته دليل الكائن مرة أخرى إلى سمة كونسيستينسيجويد مسدس في "Active Directory" على أماكن العمل.</span><span class="sxs-lookup"><span data-stu-id="3b77d-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="3b77d-108">بعد أن يتم نشر السمة كونسيستينسيجويد مسدس أو الاتصال الإعلان Azure ثم يصدر الكائن لإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="3b77d-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="3b77d-109">**ملاحظة:** مرة داخلي استيراد كائن الإعلان إلى Azure الإعلان الاتصال (أي، المستوردة إلى "مساحة موصل" الإعلان والمرتقب في Metaverse)، لا يمكن تغيير قيمته سورسينتشور بعد الآن.</span><span class="sxs-lookup"><span data-stu-id="3b77d-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="3b77d-110">لتعيين القيمة سورسينتشور للداخلي نظراً لإعلان الكائن، قم بتكوين سمة كونسيستينسيجويد مسدس به قبل استيرادها إلى الاتصال الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="3b77d-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="3b77d-111">لمزيد من المعلومات حول سورسينتشور وكونسيستينسيجويد، أرجع إلى ما يلي: [أزور الاتصال الإعلان: مفاهيم التصميم](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="3b77d-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

