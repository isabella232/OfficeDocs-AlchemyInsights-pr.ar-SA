---
title: كونسيستينسيجويد/سورسينتشور السلوك
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273141"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="9aa69-102">كونسيستينسيجويد/سورسينتشور السلوك</span><span class="sxs-lookup"><span data-stu-id="9aa69-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="9aa69-p101">الاتصال الإعلان أزور (الإصدار 1.1.524.0 وبعد) يسهل استخدام مسدس كونسيستينسيجويد كسمة سورسيانتشور الآن. عند استخدام هذه الميزة، Azure الإعلان الاتصال تلقائياً بتكوين قواعد المزامنة إلى:</span><span class="sxs-lookup"><span data-stu-id="9aa69-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="9aa69-p102">استخدام مسدس كونسيستينسيجويد كسمة سورسينتشور لكائنات المستخدم. يتم استخدام دليل الكائن لأنواع الكائنات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="9aa69-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="9aa69-p103">لأي إعطاء الداخلي المستخدم الإعلان الكائن الذي سمته مسدس كونسيستينسيجويد لا يكتب الاتصال الإعلان المعممة، Azure قيمته دليل الكائن مرة أخرى إلى سمة كونسيستينسيجويد مسدس في "Active Directory" على أماكن العمل. بعد أن يتم نشر السمة كونسيستينسيجويد مسدس أو الاتصال الإعلان Azure ثم يصدر الكائن لإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="9aa69-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="9aa69-p104">**ملاحظة:** مرة داخلي استيراد كائن الإعلان إلى Azure الإعلان الاتصال (أي، المستوردة إلى "مساحة موصل" الإعلان والمرتقب في Metaverse)، لا يمكن تغيير قيمته سورسينتشور بعد الآن. لتعيين القيمة سورسينتشور للداخلي نظراً لإعلان الكائن، قم بتكوين سمة كونسيستينسيجويد مسدس به قبل استيرادها إلى الاتصال الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="9aa69-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="9aa69-111">لمزيد من المعلومات حول سورسينتشور وكونسيستينسيجويد، أرجع إلى ما يلي: [أزور الاتصال الإعلان: مفاهيم التصميم](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="9aa69-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

