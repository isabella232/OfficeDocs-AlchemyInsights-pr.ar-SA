---
title: 646 كيفيه تكوين AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704476"
---
# <a name="configure-sync-features"></a><span data-ttu-id="0fd79-102">تكوين ميزات المزامنة</span><span class="sxs-lookup"><span data-stu-id="0fd79-102">Configure sync features</span></span>

<span data-ttu-id="0fd79-103">يتضمن Azure AD Connect العديد من الميزات التي يتم تمكينها بشكل افتراضي ، أو يمكنك تمكينها لاحقا.</span><span class="sxs-lookup"><span data-stu-id="0fd79-103">Azure AD Connect includes several features that are enabled by default, or that you can enable later.</span></span> <span data-ttu-id="0fd79-104">تتطلب بعض الميزات تكوين إضافي في بيئات معينه.</span><span class="sxs-lookup"><span data-stu-id="0fd79-104">Some features require additional configuration in specific environments.</span></span>

- <span data-ttu-id="0fd79-105">حدود [التصفية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) يتم مزامنة العناصر إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0fd79-105">[Filtering](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) limits the objects are synchronized to Azure AD.</span></span> <span data-ttu-id="0fd79-106">بشكل افتراضي ، تتم مزامنة كل المستخدمين وجات الاتصال والمجموعات وحسابات الكمبيوتر في Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0fd79-106">By default, all users, contacts, groups, and Windows 10 computer accounts are synchronized.</span></span> <span data-ttu-id="0fd79-107">يمكنك تضمين كائنات أو استبعادها استنادا إلى المجالات أو الأووس أو السمات الأخرى.</span><span class="sxs-lookup"><span data-stu-id="0fd79-107">You can include or exclude objects based on domains, OUs, or other attributes.</span></span>

- <span data-ttu-id="0fd79-108">يقوم " [مزامنة" تجزئه كلمه المرور](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) بمزامنة تجزئه كلمه المرور من active directory المحلي إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="0fd79-108">[Password hash synchronization](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) synchronizes the password hash from the on-premises Active Directory to Azure AD.</span></span> <span data-ttu-id="0fd79-109">يسمح هذا باداره كلمه المرور في موقع واحد ، ولكن استخدام نفس كلمه المرور في كل من البيئات المحلية والسحابية.</span><span class="sxs-lookup"><span data-stu-id="0fd79-109">This allows password management in one location, but use of the same password in both on-premises and cloud environments.</span></span> <span data-ttu-id="0fd79-110">لان Active Directory هو المصدر الموثوق ، يمكنك استخدام نهج كلمه المرور الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="0fd79-110">Because Active Directory is the authoritative source, you can use your own password policies.</span></span>

- <span data-ttu-id="0fd79-111">تسمح [أعاده تعيين كلمه مرور الخدمة الذاتية (سبر)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) للمستخدمين باعاده تعيين كلمات المرور الخاصة بهم في السحابة مع استمرار تطبيق نهج كلمه المرور المحلية.</span><span class="sxs-lookup"><span data-stu-id="0fd79-111">[Self-service password reset (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) allows users to reset their own passwords in the cloud while still applying your on-premises password policy.</span></span>

- <span data-ttu-id="0fd79-112">يسمح [الكتابة الخلفية للجهاز](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) باعاده كتابه الاجهزه المسجلة في Azure AD إلى active directory المحلي بحيث يمكن استخدامها للوصول الشرطي.</span><span class="sxs-lookup"><span data-stu-id="0fd79-112">[Device writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) allows registered devices in Azure AD to be written back to the on-premises Active Directory so they can be used for conditional access.</span></span>

- <span data-ttu-id="0fd79-113">[منع الحذف العرضي](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) يتم تمكينه بشكل افتراضي للمساعدة علي منع العديد من عمليات حذف الكائنات المتزامنة (أكثر من 500 كائن لكل مزامنة).</span><span class="sxs-lookup"><span data-stu-id="0fd79-113">[Prevent accidental deletes](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) is enabled by default to help prevent too many simultaneous object deletions (more than 500 objects per synchronization).</span></span> <span data-ttu-id="0fd79-114">يمكنك تغيير هذا الاعداد لتلبيه احتياجات مؤسستك.</span><span class="sxs-lookup"><span data-stu-id="0fd79-114">You can change this setting to meet the needs of your organization.</span></span>

- <span data-ttu-id="0fd79-115">يتم تمكين [الترقية التلقائية](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) بشكل افتراضي لتثبيتات express والمساعدة علي التاكد من ان إصدار Azure AD Connect حاليا دائما.</span><span class="sxs-lookup"><span data-stu-id="0fd79-115">[Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) is enabled by default for express installations and helps ensure your version of Azure AD Connect is always current.</span></span>
