---
title: استكشاف أخطاء مزامنة كلمات المرور
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390389"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="d998a-102">استكشاف أخطاء مزامنة كلمات المرور</span><span class="sxs-lookup"><span data-stu-id="d998a-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="d998a-103">لاستكشاف مشكلات فيها لم كلمات مرور متزامنة مع إصدار الاتصال الإعلان Azure 1.1.614.0 أو أحدث:</span><span class="sxs-lookup"><span data-stu-id="d998a-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="d998a-104">فتح جلسة عمل Windows PowerShell جديدة على ملقم الاتصال الإعلان Azure مع الخيار **تشغيل كمسؤول** .</span><span class="sxs-lookup"><span data-stu-id="d998a-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="d998a-105">تشغيل **مجموعة ExecutionPolicy RemoteSigned** أو **مجموعة ExecutionPolicy غير مقيد**.</span><span class="sxs-lookup"><span data-stu-id="d998a-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="d998a-106">بدء تشغيل معالج اتصال AD Azure.</span><span class="sxs-lookup"><span data-stu-id="d998a-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="d998a-107">انتقل إلى \* \* "مهام إضافية" \* \* الصفحة، حدد \* \* استكشاف \* \*، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="d998a-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="d998a-108">في الصفحة استكشاف الأخطاء وإصلاحها، انقر فوق قائمة **التشغيل لبدء استكشاف الأخطاء وإصلاحها** في PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d998a-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="d998a-109">في القائمة الرئيسية، حدد **استكشاف أخطاء مزامنة كلمات المرور**.</span><span class="sxs-lookup"><span data-stu-id="d998a-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="d998a-110">في القائمة الفرعية، حدد **"كلمة المرور المزامنة" لا تعمل على الإطلاق**.</span><span class="sxs-lookup"><span data-stu-id="d998a-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="d998a-111">**فهم نتائج مهمة استكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="d998a-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="d998a-112">مهمة استكشاف الأخطاء وإصلاحها يقوم بتنفيذ الاختبارات التالية:</span><span class="sxs-lookup"><span data-stu-id="d998a-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="d998a-113">التحقق من تمكين ميزة مزامنة كلمة المرور للمستأجر Azure الإعلان الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="d998a-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="d998a-114">التحقق من أن الملقم الاتصال الإعلان Azure ليس في إعداد وضع.</span><span class="sxs-lookup"><span data-stu-id="d998a-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="d998a-115">لكل القائمة الداخلية Active Directory الموصل (الذي يقابل إلى مجموعة تفرعات "Active Directory" موجودة):</span><span class="sxs-lookup"><span data-stu-id="d998a-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="d998a-116">التحقق من تمكين ميزة مزامنة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="d998a-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="d998a-117">البحث عن أحداث نبضات المزامنة كلمة المرور في سجلات Windows Application Event.</span><span class="sxs-lookup"><span data-stu-id="d998a-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="d998a-118">لكل مجال Active Directory ضمن موصل "خدمة active Directory" الداخلي:</span><span class="sxs-lookup"><span data-stu-id="d998a-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="d998a-119">التحقق من صحة المجال قابل من الملقم الاتصال الإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="d998a-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="d998a-120">التحقق من وجود حسابات "خدمات مجال خدمة active Directory" (AD DS) المستخدمة بواسطة موصل "خدمة active Directory" على أماكن العمل اسم المستخدم الصحيح وكلمة المرور والأذونات المطلوبة لمزامنة كلمات المرور.</span><span class="sxs-lookup"><span data-stu-id="d998a-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="d998a-121">لمزيد من استكشاف الأخطاء وإصلاحها مزامنة كلمة المرور، راجع [استكشاف الأخطاء وإصلاحها مزامنة كلمات المرور مع تزامن الاتصال الإعلان Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="d998a-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

