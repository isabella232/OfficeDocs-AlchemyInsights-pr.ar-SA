---
title: 646 كيفية تكوين آدكونيكت
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: e4ba295cd0661c3454180dd6a15895123840389e
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499657"
---
# <a name="configure-sync-features"></a><span data-ttu-id="a7b3b-102">تكوين ميزات مزامنة</span><span class="sxs-lookup"><span data-stu-id="a7b3b-102">Configure sync features</span></span>

<span data-ttu-id="a7b3b-p101">يتضمن الاتصال الإعلان azure العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو يمكنك تمكين لاحقاً. تتطلب بعض ميزات تكوين إضافية في بيئات محددة.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-p101">Azure AD Connect includes several features that are enabled by default, or that you can enable later. Some features require additional configuration in specific environments.</span></span>
  
- <span data-ttu-id="a7b3b-p102">تتم مزامنة حدود [تصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) الكائنات لإعلان Azure. بشكل افتراضي، كافة المستخدمين، جهات اتصال، مجموعات، و Windows 10 حسابات كمبيوتر تتم مزامنة. يمكنك تضمين أو استبعاد الكائنات التي تستند إلى مجالات أو وحدات تنظيمية أو السمات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-p102">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD. By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized. You can include or exclude objects based on domains, OUs, or other attributes.</span></span> 
    
- <span data-ttu-id="a7b3b-p103">مزامنة [المزامنة تجزئة كلمة مرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) كلمة مرور التجزئة من "Active Directory" الداخلي لإعلان Azure. يسمح هذا إدارة كلمة المرور في موقع واحد، لكن باستخدام نفس كلمة المرور في كل من المحلي وبيئات مجموعة النظراء. نظراً لأن "خدمة active Directory" مصدر موثوق به، يمكنك استخدام نهج كلمة المرور الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-p103">[Password hash syncronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD. This allows password management in one location, but use of the same password in both on-premises and cloud environments. Because Active Directory is the authoritative source, you can use your own password policies.</span></span> 
    
- <span data-ttu-id="a7b3b-111">[إعادة تعيين كلمة المرور الخدمة الذاتية (صبر)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) يسمح للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في مجموعة النظراء أثناء استمرار تطبيق نهج كلمة المرور المحلية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span> 
    
- <span data-ttu-id="a7b3b-112">يسمح [الجهاز إعادة الكتابة](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) الأجهزة المسجلة في AD Azure إعادة كتابته في خدمة "active Directory" الداخلي حيث يمكن استخدامها للوصول المشروط.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span> 
    
- <span data-ttu-id="a7b3b-p104">يتم تمكين [العرضي منع الحذف](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) بشكل افتراضي لمنع حذف الكائنات المتزامنة كثيرة جداً (أكثر من 500 الكائنات كل المزامنة). يمكنك تغيير هذا الإعداد لتلبية احتياجات المؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-p104">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization). You can change this setting to meet the needs of your organization.</span></span> 
    
- <span data-ttu-id="a7b3b-115">تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) افتراضياً للتثبيتات السريعة ويضمن دائماً الإصدار الخاص بك من الاتصال Azure الإعلان الحالي.</span><span class="sxs-lookup"><span data-stu-id="a7b3b-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span> 
    

