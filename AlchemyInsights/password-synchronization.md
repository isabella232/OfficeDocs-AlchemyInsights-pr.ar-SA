---
title: مزامنة كلمة المرور
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480859"
---
# <a name="password-synchronization"></a><span data-ttu-id="17733-102">مزامنة كلمة المرور</span><span class="sxs-lookup"><span data-stu-id="17733-102">Password synchronization</span></span>

<span data-ttu-id="17733-103">**لا تعمل مزامنة كلمة المرور المتزامنة على الإطلاق**</span><span class="sxs-lookup"><span data-stu-id="17733-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="17733-104">بعض المشاكل الشائعة التي يواجهها العملاء عند عدم عمل مزامنة كلمة المرور المتزامنة هي:</span><span class="sxs-lookup"><span data-stu-id="17733-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="17733-105">لا يتم منح حساب Active Directory الذي يستخدمه Azure AD Connect  للتواصل مع Active  Directory في الموقع "تغييرات دليل النسخ المتماثل" و"نسخ الدليل المتماثل" يغير كل الأذونات المطلوبة لمزامنة كلمة المرور - يجب إصلاح ذلك من خلال منح هذه الأذونات لحساب Active Directory.</span><span class="sxs-lookup"><span data-stu-id="17733-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="17733-106">يتم تعطيل مزامنة كلمة المرور بعد أن يقوم المسؤول بتغيير  أسلوب المستخدم Sign-In من "مزامنة كلمة المرور" إلى خيار آخر مثل "الاتحاد مع **AD FS"** في معالج Azure AD Connect - يمكنك إصلاح ذلك من خلال إعادة تمكين ميزة مزامنة كلمة المرور في معالج Azure AD Connect. </span><span class="sxs-lookup"><span data-stu-id="17733-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="17733-107">مشكلة في الاتصال مع Active Directory في الموقع.</span><span class="sxs-lookup"><span data-stu-id="17733-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="17733-108">على سبيل المثال، يتعذر على Azure AD Connect [](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) الوصول إلى بعض وحدات التحكم بالمجال، أو يتم حظر المنافذ المطلوبة بواسطة جدار الحماية - يجب إصلاح ذلك من خلال ضمان عمل الاتصال بين خادم Azure AD Connect و Active Directory في الموقع بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="17733-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="17733-109">خادم Azure AD Connect موجود حاليا في وضع الترحيل، مما يؤدي إلى عدم تمكن الخادم من الوصول إلى تقسمات كلمة المرور - لاتباع الخطوات الموضحة في مزامنة كلمة المرور في القسم وإصلاحها مع مزامنة [Azure AD Connect -](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)لا تتم مزامنة أي كلمات مرور.</span><span class="sxs-lookup"><span data-stu-id="17733-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="17733-110">**لا تعمل مزامنة كلمة المرور المتزامنة مع بعض المستخدمين**</span><span class="sxs-lookup"><span data-stu-id="17733-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="17733-111">إذا لاحظت عدم مزامنة كلمة المرور للمستخدم، فاستخدم  مهمة استكشاف الأخطاء وإصلاحها في Azure AD Connect للتحقق من المشكلة وحلها.</span><span class="sxs-lookup"><span data-stu-id="17733-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="17733-112">تنفيذ المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="17733-112">Perform the following tasks:</span></span>

    <span data-ttu-id="17733-113">أ.</span><span class="sxs-lookup"><span data-stu-id="17733-113">a.</span></span> [<span data-ttu-id="17733-114">تشغيل مهمة استكشاف الأخطاء وإصلاحها في المعالج</span><span class="sxs-lookup"><span data-stu-id="17733-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="17733-115">ب.</span><span class="sxs-lookup"><span data-stu-id="17733-115">b.</span></span> [<span data-ttu-id="17733-116">استخدام الأمر cmdlet الخاص بابتكار الأخطاء وإصلاحها للتحقق من مشكلة مزامنة كلمة المرور لاستخدام معين</span><span class="sxs-lookup"><span data-stu-id="17733-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="17733-117">يتم تمكين كائن مستخدم Active Directory في الموقع، حيث يجب على المستخدم تغيير كلمة المرور **في خيار تسجيل** الدخول التالي.</span><span class="sxs-lookup"><span data-stu-id="17733-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="17733-118">عند تمكين هذا الخيار، يتم تعيين كلمة مرور مؤقتة للمستخدم وستطالب بتغيير كلمة المرور في تسجيل الدخول التالي.</span><span class="sxs-lookup"><span data-stu-id="17733-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="17733-119">لا يقوم Azure AD Connect بمزامنة كلمات المرور المؤقتة إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17733-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="17733-120">لحل المشكلة أعلاه، تنفيذ أي من المهام التالية:</span><span class="sxs-lookup"><span data-stu-id="17733-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="17733-121">اطلب من المستخدم تسجيل الدخول إلى التطبيق المحلي (على سبيل المثال، سطح مكتب Windows) وتغيير كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="17733-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="17733-122">سيتم مزامنة كلمة المرور الجديدة إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="17733-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="17733-123">يجب أن يقوم مسؤول بتحديث كلمة مرور المستخدم دون تمكين الخيار الذي يجب على المستخدم تغيير كلمة المرور عند تسجيل الدخول التالي، ومشاركة كلمة المرور الجديدة مع المستخدم.</span><span class="sxs-lookup"><span data-stu-id="17733-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="17733-124">لم يتم تكوين كائن مستخدم Active  Directory في الموقع بشكل صحيح لمزامنة الكائنات أو مزامنة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="17733-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="17733-125">استكشاف هذه المشكلة وإصلاحها، اتبع الخطوات الموضحة في مزامنة كلمة المرور المتزامنة مع مزامنة [Azure AD Connect وإصلاحها.](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)</span><span class="sxs-lookup"><span data-stu-id="17733-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







