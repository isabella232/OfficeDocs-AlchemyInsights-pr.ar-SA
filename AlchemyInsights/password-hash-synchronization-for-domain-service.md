---
title: مزامنة كلمة المرور المتزامنة لخدمة المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177352"
---
# <a name="password-hash-synchronization-for-domain-service"></a><span data-ttu-id="bc58f-102">مزامنة كلمة المرور المتزامنة لخدمة المجال</span><span class="sxs-lookup"><span data-stu-id="bc58f-102">Password hash synchronization for domain service</span></span>

<span data-ttu-id="bc58f-103">**إذا كان مثيل Azure AD DS يطالبك بتمكين مزامنة كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="bc58f-103">**If your Azure AD DS instance is prompting you to enable password hash synchronization**</span></span>

<span data-ttu-id="bc58f-104">تواجه سيناريو تقوم فيه بتشغيل بيئة مختلطة مع مزامنة المستخدمين من بيئة Azure Active Directory Domain Services (AD DS) المحلية.</span><span class="sxs-lookup"><span data-stu-id="bc58f-104">You encounter a scenario in which you are running a hybrid environment with users synchronizing from an on-premises Azure Active Directory Domain Services (AD DS) environment.</span></span> <span data-ttu-id="bc58f-105">يتم مواجهة هذا السيناريو على الرغم من مزامنة كلمة المرور المتزامنة بين AD DS ومستأجر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bc58f-105">This scenario is encountered despite you having password hash synchronization from the on-premises AD DS to your Azure AD tenant.</span></span>

<span data-ttu-id="bc58f-106">**السبب**</span><span class="sxs-lookup"><span data-stu-id="bc58f-106">**Cause**</span></span>

<span data-ttu-id="bc58f-107">يحدث هذا الأمر لأن Azure AD Connect لا يقوم بشكل افتراضي بمزامنة كلمات مرور Azure AD DS القديمة في New Technology Manager (NTLM) وKerberos.</span><span class="sxs-lookup"><span data-stu-id="bc58f-107">This is happening because Azure AD Connect by default does not synchronize legacy New Technology LAN Manager (NTLM) and Kerberos password hashes that are needed for Azure AD DS.</span></span>

<span data-ttu-id="bc58f-108">**الحل البديل**</span><span class="sxs-lookup"><span data-stu-id="bc58f-108">**Workaround**</span></span> 

<span data-ttu-id="bc58f-109">قد تحتاج إلى تكوين Azure AD Connect لمزامنة كلمات المرور المتزامنة المطلوبة لمصادقة NTLM وKerberos.</span><span class="sxs-lookup"><span data-stu-id="bc58f-109">You would need to configure Azure AD Connect to synchronize those password hashes required for NTLM and Kerberos authentication.</span></span>

<span data-ttu-id="bc58f-110">بعد تكوين Azure AD Connect، يتزامن أيضا حدث إنشاء حساب أو تغيير كلمة مرور في الموقع مع Azure AD.</span><span class="sxs-lookup"><span data-stu-id="bc58f-110">After Azure AD Connect is configured, an on-premises account creation or password change event also then synchronizes the legacy password hashes to Azure AD.</span></span> <span data-ttu-id="bc58f-111">الرجاء الاطلاع [هنا](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) للحصول على مزيد من المعلومات حول ذلك للحصول على إرشادات حول كيفية تمكين مزامنة كلمة المرور في بيئات Azure AD DS المختلطة.</span><span class="sxs-lookup"><span data-stu-id="bc58f-111">Please see [here](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) for more information on this and for guidance on how to enable password synchronization in Azure AD DS hybrid environments.</span></span>