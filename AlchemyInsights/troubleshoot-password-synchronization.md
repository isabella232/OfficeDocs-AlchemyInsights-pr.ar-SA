---
title: استكشاف مزامنة كلمة المرور وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732497"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="a4823-102">استكشاف مزامنة كلمة المرور وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="a4823-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="a4823-103">لاستكشاف المشكلات التي لا تتم فيها مزامنة كلمات المرور مع إصدار Azure AD Connect 1.1.614.0 أو أحدث:</span><span class="sxs-lookup"><span data-stu-id="a4823-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="a4823-104">افتح جلسة عمل Windows PowerShell جديدة على خادم Azure AD Connect مع خيار **التشغيل كمسؤول.**</span><span class="sxs-lookup"><span data-stu-id="a4823-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="a4823-105">تشغيل **مجموعة التنفيذنهج عن بعد موقعة** أو **مجموعة التنفيذسياسة غير المقيدة**.</span><span class="sxs-lookup"><span data-stu-id="a4823-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="a4823-106">بدء تشغيل معالج Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a4823-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="a4823-107">انتقل إلى صفحة **المهام الإضافية،** وحدد **استكشاف الأخطاء وإصلاحها،** وانقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="a4823-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="a4823-108">في صفحة استكشاف الأخطاء وإصلاحها، انقر فوق تشغيل لبدء قائمة **استكشاف الأخطاء وإصلاحها** في PowerShell.</span><span class="sxs-lookup"><span data-stu-id="a4823-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="a4823-109">في القائمة الرئيسية، حدد **استكشاف مزامنة كلمة المرور وإصلاحها**.</span><span class="sxs-lookup"><span data-stu-id="a4823-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="a4823-110">في القائمة الفرعية، حدد **مزامنة كلمة المرور لا يعمل على الإطلاق**.</span><span class="sxs-lookup"><span data-stu-id="a4823-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="a4823-111">**فهم نتائج مهمة استكشاف الأخطاء وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="a4823-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="a4823-112">تنفيذ مهمة استكشاف الأخطاء وإصلاحها الشيكات التالية:</span><span class="sxs-lookup"><span data-stu-id="a4823-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="a4823-113">التحقق من تمكين ميزة مزامنة كلمة المرور لمستأجر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="a4823-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="a4823-114">التحقق من أن ملقم Azure AD Connect ليس في وضع التدريج.</span><span class="sxs-lookup"><span data-stu-id="a4823-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="a4823-115">لكل موصل "الدليل النشط" الموجود في الموقع (الذي يتوافق مع مجموعة تفرعات "الدليل النشط" الموجودة):</span><span class="sxs-lookup"><span data-stu-id="a4823-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="a4823-116">التحقق من تمكين ميزة مزامنة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="a4823-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="a4823-117">البحث عن أحداث نبضات قلب مزامنة كلمة المرور في سجلات أحداث تطبيق Windows.</span><span class="sxs-lookup"><span data-stu-id="a4823-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="a4823-118">لكل مجال "الدليل النشط" ضمن موصل "الدليل النشط" الداخلي:</span><span class="sxs-lookup"><span data-stu-id="a4823-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="a4823-119">التحقق من أن المجال يمكن الوصول إليه من خادم Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="a4823-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="a4823-120">التحقق من صحة أن حسابات خدمات مجال الدليل النشط (AD DS) المستخدمة من قبل موصل الدليل النشط الداخلي لديها اسم المستخدم الصحيح وكلمة المرور والأذونات المطلوبة لمزامنة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="a4823-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="a4823-121">لمزيد من المساعدة في استكشاف مزامنة كلمة المرور [وإصلاحها، راجع استكشاف مزامنة كلمة المرور وإصلاحها باستخدام مزامنة Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="a4823-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  