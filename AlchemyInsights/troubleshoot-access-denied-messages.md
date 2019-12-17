---
title: استكشاف أخطاء رسائل "رفض الوصول" وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 05d12aee49b449e8a29e84021b41298fb9983859
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050692"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="83172-102">استكشاف أخطاء رسائل "رفض الوصول" وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="83172-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="83172-103">إذا حصل أحد الأشخاص علي رسالة "تم رفض الوصول" إلى مجلد مشترك في SharePoint ، فقد يكون مسؤول مجموعه الموقع قد قام بتمكين "وضع تامين اذن المستخدم المحدود الوصول".</span><span class="sxs-lookup"><span data-stu-id="83172-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="83172-104">لإيقاف تشغيل هذا:</span><span class="sxs-lookup"><span data-stu-id="83172-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="83172-105">استعرض لوصول إلى الموقع ، انقر فوق الرمز إعدادات ، ثم انقر فوق **إعدادات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="83172-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="83172-106">ضمن **أداره مجموعه الموقع**، انقر فوق **ميزات مجموعه الموقع**.</span><span class="sxs-lookup"><span data-stu-id="83172-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="83172-107">بجوار **وضع تامين اذن المستخدم الوصول المحدود**، انقر فوق **إلغاء تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="83172-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="83172-108">يمكن ان تحدث رسالة "رفض الوصول" أيضا للمجلدات المشتركة إذا كان الموقع موقع نشر.</span><span class="sxs-lookup"><span data-stu-id="83172-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="83172-109">للحصول علي معلومات ، راجع [رفض الوصول عند الوصول إلى مجلد مشترك](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="83172-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="83172-110">إذا حصل شخص ما علي رسالة "تم رفض الوصول" عند محاولة عرض طلبات الوصول ، يحتاج المستخدم إلى اضافته اما كمسؤول مجموعه موقع أو كعضو في مجموعه المالكين للموقع.</span><span class="sxs-lookup"><span data-stu-id="83172-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="83172-111">لمزيد من المعلومات ، راجع [قائمه رفض الوصول إلى طلبات الوصول](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="83172-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="83172-112">إذا حصل مستخدم علي رسالة "تم رفض الوصول" بعد ازالتها من Active Directory المحلي ثم اضافتها مره أخرى ، راجع [رفض الوصول عند مزامنة حساب مستخدم إلى Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="83172-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

