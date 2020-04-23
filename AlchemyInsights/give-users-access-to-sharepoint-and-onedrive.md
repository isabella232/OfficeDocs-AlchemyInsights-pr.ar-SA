---
title: منح المستخدمين حق الوصول إلى SharePoint وOneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 0bdc2fa97ad1fe8b3280411babaaf2bd685a644d
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43721683"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="d2b1f-102">منح المستخدمين حق الوصول إلى SharePoint وOneDrive</span><span class="sxs-lookup"><span data-stu-id="d2b1f-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="d2b1f-103">إذا كان موقع OneDrive أو SharePoint غير متوفر للعديد من المستخدمين الذين سبق لهم الوصول، فقد تكون هناك مشكلة في الخدمة المؤقتة.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="d2b1f-104">التحقق من لوحة معلومات صحة الخدمة</span><span class="sxs-lookup"><span data-stu-id="d2b1f-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="d2b1f-105">إذا كنت تريد أن يتمكن الأشخاص في مؤسستك من تسجيل الدخول واستخدام SharePoint و OneDrive، فستحتاج إلى إضافة حسابات لهم والتأكد من حصولهم على ترخيص يتيح لهم الوصول إلى SharePoint و OneDrive.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="d2b1f-106">أسهل طريقة لإضافة المستخدمين هي في مركز إدارة Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="d2b1f-107">انتقل إلى [صفحة المستخدمين النشطين في مركز إدارة Microsoft 365،](https://portal.office.com/adminportal/home#/users)ثم انقر فوق **إضافة مستخدم**.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="d2b1f-108">قم بتعبئة المعلومات الخاصة بالمستخدم، وتأكد من أنه بموجب **تراخيص المنتج،** يتم تعيين ترخيص وتحديد **SharePoint Online.**</span><span class="sxs-lookup"><span data-stu-id="d2b1f-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="d2b1f-109">لاحظ أنه إذا سمحت بالمشاركة الخارجية في مؤسستك، يمكن للمستخدمين مشاركة محتوى SharePoint وOneDrive مع أشخاص خارج المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="d2b1f-110">لا تحتاج إلى منح تراخيص المستخدمين الخارجيين هؤلاء.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="d2b1f-111">لا تحتاج أيضًا إلى إضافة حسابات لها، ما لم يتم تعيين المشاركة إلى "المستخدمين الخارجيين الموجودين فقط".</span><span class="sxs-lookup"><span data-stu-id="d2b1f-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="d2b1f-112">في هذه الحالة، إذا لم يكن الأشخاص في دليل مؤسستك، فستحتاج إلى إضافتهم كمستخدمين ضيوف في مركز إدارة Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d2b1f-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

