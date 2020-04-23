---
title: 646 كيفية تكوين AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722508"
---
# <a name="configure-sync-features"></a><span data-ttu-id="fe80b-102">تكوين ميزات المزامنة</span><span class="sxs-lookup"><span data-stu-id="fe80b-102">Configure sync features</span></span>

<span data-ttu-id="fe80b-103">يتضمن Azure AD Connect العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو التي يمكنك تمكينها لاحقًا.</span><span class="sxs-lookup"><span data-stu-id="fe80b-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="fe80b-104">تتطلب بعض الميزات تكوينًا إضافيًا في بيئات معينة.</span><span class="sxs-lookup"><span data-stu-id="fe80b-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="fe80b-105">[تصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) حدود تتم مزامنة الكائنات إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe80b-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="fe80b-106">بشكل افتراضي، تتم مزامنة كافة المستخدمين وجهات الاتصال والمجموعات وحسابات الكمبيوتر Windows 10.</span><span class="sxs-lookup"><span data-stu-id="fe80b-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="fe80b-107">يمكنك تضمين الكائنات أو استبعادها استنادًا إلى المجالات أو OUs أو السمات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="fe80b-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="fe80b-108">[مزامنة تجزئة كلمة المرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) مزامنة تجزئة كلمة المرور من الدليل النشط الداخلي إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="fe80b-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="fe80b-109">يسمح هذا بإدارة كلمة المرور في موقع واحد، ولكن استخدام نفس كلمة المرور في كل من البيئات الداخلية والسحابية.</span><span class="sxs-lookup"><span data-stu-id="fe80b-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="fe80b-110">لأن "الدليل النشط" هو المصدر الموثوق به، يمكنك استخدام نُهج كلمة المرور الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="fe80b-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="fe80b-111">تسمح [إعادة تعيين كلمة مرور الخدمة الذاتية (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في السحابة أثناء تطبيق نهج كلمة المرور الداخلي الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="fe80b-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="fe80b-112">يسمح [رد كتابة الجهاز](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) بكتابة الأجهزة المسجلة في Azure AD مرة أخرى إلى الدليل النشط الداخلي بحيث يمكن استخدامها للوصول المشروط.</span><span class="sxs-lookup"><span data-stu-id="fe80b-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="fe80b-113">منع [حذف عرضي](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) يتم تمكين بشكل افتراضي للمساعدة في منع حذف الكائنات في وقت واحد كثيرة جداً (أكثر من 500 كائن لكل مزامنة).</span><span class="sxs-lookup"><span data-stu-id="fe80b-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="fe80b-114">يمكنك تغيير هذا الإعداد لتلبية احتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="fe80b-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="fe80b-115">يتم تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) بشكل افتراضي للتثبيتات السريعة وتساعد على ضمان تحديث إصدار Azure AD Connect دائمًا.</span><span class="sxs-lookup"><span data-stu-id="fe80b-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
