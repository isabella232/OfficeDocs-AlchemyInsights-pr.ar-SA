---
title: 646 كيفية تكوين آدكوننيكت
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385316"
---
# <a name="configure-sync-features"></a><span data-ttu-id="74a18-102">تكوين ميزات مزامنة</span><span class="sxs-lookup"><span data-stu-id="74a18-102">Configure sync features</span></span>

<span data-ttu-id="74a18-103">يتضمن الاتصال الإعلان azure العديد من الميزات التي يتم تمكينها بشكل افتراضي، أو يمكنك تمكين لاحقاً.</span><span class="sxs-lookup"><span data-stu-id="74a18-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="74a18-104">تتطلب بعض ميزات تكوين إضافية في بيئات محددة.</span><span class="sxs-lookup"><span data-stu-id="74a18-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="74a18-105">تتم مزامنة حدود [تصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) الكائنات لإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="74a18-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="74a18-106">بشكل افتراضي، كافة المستخدمين، جهات اتصال، مجموعات، و Windows 10 حسابات كمبيوتر تتم مزامنة.</span><span class="sxs-lookup"><span data-stu-id="74a18-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="74a18-107">يمكنك تضمين أو استبعاد الكائنات التي تستند إلى مجالات أو وحدات تنظيمية أو السمات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="74a18-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="74a18-108">مزامنة [المزامنة تجزئة كلمة مرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) كلمة مرور التجزئة من "Active Directory" الداخلي لإعلان Azure.</span><span class="sxs-lookup"><span data-stu-id="74a18-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="74a18-109">يسمح هذا إدارة كلمة المرور في موقع واحد، لكن باستخدام نفس كلمة المرور في كل من المحلي وبيئات مجموعة النظراء.</span><span class="sxs-lookup"><span data-stu-id="74a18-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="74a18-110">نظراً لأن "خدمة active Directory" مصدر موثوق به، يمكنك استخدام نهج كلمة المرور الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="74a18-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="74a18-111">[إعادة تعيين كلمة المرور الخدمة الذاتية (صبر)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) يسمح للمستخدمين بإعادة تعيين كلمات المرور الخاصة بهم في مجموعة النظراء أثناء استمرار تطبيق نهج كلمة المرور المحلية الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="74a18-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="74a18-112">يسمح [الجهاز إعادة الكتابة](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) الأجهزة المسجلة في AD Azure إعادة كتابته في خدمة "active Directory" الداخلي حيث يمكن استخدامها للوصول المشروط.</span><span class="sxs-lookup"><span data-stu-id="74a18-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="74a18-113">يتم تمكين [العرضي منع الحذف](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) بشكل افتراضي لمنع حذف الكائنات المتزامنة كثيرة جداً (أكثر من 500 الكائنات كل المزامنة).</span><span class="sxs-lookup"><span data-stu-id="74a18-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="74a18-114">يمكنك تغيير هذا الإعداد لتلبية احتياجات المؤسسة الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="74a18-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="74a18-115">تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) افتراضياً للتثبيتات السريعة ويضمن دائماً الإصدار الخاص بك من الاتصال Azure الإعلان الحالي.</span><span class="sxs-lookup"><span data-stu-id="74a18-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
