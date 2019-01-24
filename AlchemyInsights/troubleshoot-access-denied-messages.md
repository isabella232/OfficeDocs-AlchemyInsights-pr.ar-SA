---
title: استكشاف أخطاء رسائل "رفض الوصول"
ms.author: kaarins
author: kaarins
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 3973f5bf584343d3353e7389f22bc727827b5c35
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29455413"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="c0985-102">استكشاف أخطاء رسائل "رفض الوصول"</span><span class="sxs-lookup"><span data-stu-id="c0985-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="c0985-p101">إذا كان شخص ما حصلت على رسالة "تم رفض الوصول" إلى مجلد مشترك، مسؤول مجموعة الموقع ربما قمت بتمكين "الوصول المحدود المستخدم إذن تأمين الوضع." لإيقاف تشغيل هذا:</span><span class="sxs-lookup"><span data-stu-id="c0985-p101">If someone got an "Access Denied" message to a shared folder, the site collection administrator might have enabled "Limited-access user permission lockdown mode." To turn this off:</span></span> 
  
1. <span data-ttu-id="c0985-105">استعرض للوصول إلى الموقع وانقر فوق الرمز إعدادات ثم انقر فوق **إعدادات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="c0985-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="c0985-106">ضمن **إدارة مجموعة الموقع**، انقر فوق **ميزات مجموعة الموقع**.</span><span class="sxs-lookup"><span data-stu-id="c0985-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="c0985-107">إلى جانب **وضع تأمين إذن المستخدم الوصول المحدود**، انقر فوق **إلغاء التنشيط**.</span><span class="sxs-lookup"><span data-stu-id="c0985-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="c0985-p102">أيضا يمكن أن يحدث رسالة "رفض الوصول" للمجلدات المشتركة إذا كان الموقع عبارة عن موقع نشر. لمزيد من المعلومات، راجع [رفض الوصول عند محاولة الوصول إلى مجلد مشترك](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="c0985-p102">An Access Denied message can also occur for shared folders if the site is a publishing site. For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="c0985-p103">إذا كان شخص حصلت على رسالة "تم رفض الوصول" عند محاولة عرض طلبات الوصول، يحتاج المستخدم المراد إضافته كمسؤول مجموعة موقع أو عضو مجموعة مالكي الموقع. لمزيد من المعلومات، راجع [رفض الوصول إلى قائمة "طلبات الوصول"](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="c0985-p103">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site. For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="c0985-112">إذا حصل مستخدم على رسالة "تم رفض الوصول" بعد إزالة من Active Directory الداخلي وإضافتها مرة أخرى، راجع [رفض الوصول عند حساب مستخدم تمت مزامنته مع Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="c0985-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Office 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

