---
title: استكشاف أخطاء الوصول الرسائل المرفوضة
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 1930edcfd14acc48ea77b66e2793654a3e6332cc
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759787"
---
# <a name="troubleshoot-access-denied-messages"></a><span data-ttu-id="7f140-102">استكشاف أخطاء الوصول الرسائل المرفوضة</span><span class="sxs-lookup"><span data-stu-id="7f140-102">Troubleshoot Access Denied messages</span></span>

<span data-ttu-id="7f140-103">إذا حصل شخص ما على رسالة "رفض الوصول" إلى مجلد مشترك في SharePoint، فقد يكون مسؤول مجموعة الموقع قد قام بتمكين "وضع تأمين إذن المستخدم المحدود الوصول".</span><span class="sxs-lookup"><span data-stu-id="7f140-103">If someone got an "Access Denied" message to a shared folder in SharePoint, the site collection administrator might have enabled "Limited-access user permission lockdown mode."</span></span> <span data-ttu-id="7f140-104">لإيقاف تشغيل هذا:</span><span class="sxs-lookup"><span data-stu-id="7f140-104">To turn this off:</span></span> 
  
1. <span data-ttu-id="7f140-105">استعرض إلى الموقع، انقر فوق رمز الإعدادات، ثم انقر فوق **إعدادات الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7f140-105">Browse to the site, click the Settings icon, and then click **Site Settings**.</span></span>
    
2. <span data-ttu-id="7f140-106">ضمن **إدارة مجموعة الموقع،** انقر فوق **ميزات مجموعة الموقع**.</span><span class="sxs-lookup"><span data-stu-id="7f140-106">Under **Site Collection Administration**, click **Site collection features**.</span></span>
    
3. <span data-ttu-id="7f140-107">بجوار **وضع تأمين إذن المستخدم المحدود الوصول**، انقر فوق إلغاء **تنشيط**.</span><span class="sxs-lookup"><span data-stu-id="7f140-107">Next to **Limited-access user permission lockdown mode**, click **Deactivate**.</span></span>
    
<span data-ttu-id="7f140-108">يمكن أن تحدث رسالة رفض الوصول أيضاً للمجلدات المشتركة إذا كان الموقع موقع نشر.</span><span class="sxs-lookup"><span data-stu-id="7f140-108">An Access Denied message can also occur for shared folders if the site is a publishing site.</span></span> <span data-ttu-id="7f140-109">للحصول على معلومات، راجع [رفض الوصول عند الوصول إلى مجلد مشترك](https://go.microsoft.com/fwlink/?linkid=2004317).</span><span class="sxs-lookup"><span data-stu-id="7f140-109">For info, see [Access Denied when accessing a shared folder](https://go.microsoft.com/fwlink/?linkid=2004317).</span></span>
  
<span data-ttu-id="7f140-110">إذا حصل شخص ما على رسالة "رفض الوصول" عند محاولة عرض طلبات الوصول، يجب إضافة المستخدم كمسؤول مجموعة موقع أو عضو في مجموعة المالكين للموقع.</span><span class="sxs-lookup"><span data-stu-id="7f140-110">If a someone got an "Access Denied" message when trying to view access requests, the user needs to be added as either a site collection administrator or a member of the Owners group for the site.</span></span> <span data-ttu-id="7f140-111">لمزيد من المعلومات، راجع [قائمة طلبات الوصول المرفوضة](https://go.microsoft.com/fwlink/?linkid=2004220).</span><span class="sxs-lookup"><span data-stu-id="7f140-111">For more info, see [Access Denied to Access Requests list](https://go.microsoft.com/fwlink/?linkid=2004220).</span></span>
  
<span data-ttu-id="7f140-112">إذا حصل أحد المستخدمين على رسالة "رفض الوصول" بعد إزالتها من "الدليل النشط" في الموقع ثم إضافتها مرة أخرى، راجع [رفض الوصول عند مزامنة حساب مستخدم إلى Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span><span class="sxs-lookup"><span data-stu-id="7f140-112">If a user got an "Access Denied" message after they were removed from Active Directory on-premises and then added back, see [Access Denied when a user account is synced to Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2004318).</span></span>
  

