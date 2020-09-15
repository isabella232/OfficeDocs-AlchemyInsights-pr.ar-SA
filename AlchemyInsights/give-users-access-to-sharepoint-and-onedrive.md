---
title: منح المستخدمين حق الوصول إلى SharePoint و OneDrive
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
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: a7e9c0b7ffa5c11a2e24ee5fda6491f049f985f1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47677194"
---
# <a name="give-users-access-to-sharepoint-and-onedrive"></a><span data-ttu-id="db6a9-102">منح المستخدمين حق الوصول إلى SharePoint و OneDrive</span><span class="sxs-lookup"><span data-stu-id="db6a9-102">Give users access to SharePoint and OneDrive</span></span>

> [!NOTE]
> <span data-ttu-id="db6a9-103">إذا لم يكن موقع OneDrive أو SharePoint متوفرا لعده مستخدمين لديهم حق الوصول ، فقد تكون هناك مشكله خدمه مؤقته.</span><span class="sxs-lookup"><span data-stu-id="db6a9-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> [<span data-ttu-id="db6a9-104">التحقق من لوحه معلومات حماية الخدمة</span><span class="sxs-lookup"><span data-stu-id="db6a9-104">Check the service health dashboard</span></span>](https://portal.office.com/adminportal/home#/servicehealth)
  
<span data-ttu-id="db6a9-105">إذا كنت تريد تمكين الأشخاص في مؤسستك من تسجيل الدخول إلى SharePoint و OneDrive واستخدامهما ، ستحتاج إلى أضافه حسابات لهم والتاكد من وجود ترخيص يمنحهم حق الوصول إلى SharePoint و OneDrive.</span><span class="sxs-lookup"><span data-stu-id="db6a9-105">If you want people in your organization to be able to sign in and use SharePoint and OneDrive, you need to add accounts for them and make sure they have a license that gives them access to SharePoint and OneDrive.</span></span> <span data-ttu-id="db6a9-106">تتمثل أسهل طريقه لأضافه مستخدمين في مركز أداره Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="db6a9-106">The easiest way to add users is in the Microsoft 365 admin center.</span></span>
  
1. <span data-ttu-id="db6a9-107">انتقل إلى [صفحه المستخدمون النشطون في مركز أداره Microsoft 365](https://portal.office.com/adminportal/home#/users)، ثم انقر فوق **أضافه مستخدم**.</span><span class="sxs-lookup"><span data-stu-id="db6a9-107">Go to the [Active users page in the Microsoft 365 admin center](https://portal.office.com/adminportal/home#/users), and then click **Add a user**.</span></span>
    
2. <span data-ttu-id="db6a9-108">قم بتعبئة المعلومات الخاصة بالمستخدم ، وتاكد من انه تم تعيين ترخيص ل **SharePoint Online** ضمن **تراخيص المنتجات**.</span><span class="sxs-lookup"><span data-stu-id="db6a9-108">Fill in the information for the user, and make sure that under **Product licenses**, a license is assigned and **SharePoint Online** is selected.</span></span> 
    
<span data-ttu-id="db6a9-109">لاحظ انه إذا سمحت بالمشاركة الخارجية في مؤسستك ، فبامكان المستخدمين مشاركه محتوي SharePoint و OneDrive مع أشخاص من خارج المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="db6a9-109">Note that if you allow external sharing in your organization, users can share SharePoint and OneDrive content with people outside the organization.</span></span> <span data-ttu-id="db6a9-110">لا تحتاج إلى منح تراخيص المستخدمين الخارجيين هذه.</span><span class="sxs-lookup"><span data-stu-id="db6a9-110">You don't need to give these external users licenses.</span></span> <span data-ttu-id="db6a9-111">لا تحتاج أيضا إلى أضافه حسابات لهم ، ما لم يتم تعيين المشاركة إلى "المستخدمون الخارجيون فقط".</span><span class="sxs-lookup"><span data-stu-id="db6a9-111">You also don't need to add accounts for them, unless sharing is set to "Only existing external users."</span></span> <span data-ttu-id="db6a9-112">في هذه الحالة ، إذا لم يكن الأشخاص في دليل مؤسستك ، ستحتاج إلى اضافتهم كمستخدمين ضيوف في مركز أداره Azure AD.</span><span class="sxs-lookup"><span data-stu-id="db6a9-112">In that case, if the people aren't in your organization's directory, you need to add them as guest users in the Azure AD admin center.</span></span>
  

