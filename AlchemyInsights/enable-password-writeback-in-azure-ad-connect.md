---
title: تمكين الكتابة بكلمة مرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 2ad7568bded3c8e4832e0e433a2d715e6307e4bb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813999"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="e3e47-102">تمكين الكتابة بكلمة مرور في Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="e3e47-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="e3e47-103">لتمكين إعادة تعيين الكتابة بكلمة مرور الخدمة الذاتية، قم أولا بتمكين خيار الكتابة في Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="e3e47-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="e3e47-104">من خادم Azure AD Connect، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="e3e47-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="e3e47-105">سجل الدخول إلى خادم Azure AD Connect وابدأ معالج تكوين **Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="e3e47-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="e3e47-106">في صفحة **الترحيب،** انقر فوق **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="e3e47-107">في صفحة **المهام الإضافية،** حدد **تخصيص خيارات المزامنة**، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="e3e47-108">في صفحة **الاتصال ب Azure AD،** أدخل بيانات اعتماد المسؤول العام لمستأجر Azure، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="e3e47-109">في **صفحتي تصفية** الدلائل و **Domain/OU** Connect، انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="e3e47-110">في صفحة **الميزات الاختيارية،** حدد المربع بجانب إعادة كتابة كلمة **المرور** وانقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="e3e47-111">في الصفحة **جاهز للتكوين،** انقر فوق **تكوين** وانتظر حتى تنتهي العملية.</span><span class="sxs-lookup"><span data-stu-id="e3e47-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="e3e47-112">عندما ترى انتهاء التكوين، انقر فوق **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="e3e47-113">مع تمكين إعادة كتابة كلمة المرور في Azure AD Connect، قم بتكوين Azure AD SSPR للكتابة.</span><span class="sxs-lookup"><span data-stu-id="e3e47-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="e3e47-114">لتمكين كتابة كلمة المرور في SSPR، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="e3e47-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="e3e47-115">سجل الدخول إلى مدخل Azure باستخدام حساب مسؤول عام.</span><span class="sxs-lookup"><span data-stu-id="e3e47-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="e3e47-116">ابحث عن **Azure Active Directory** وحدده، وانقر **فوق** إعادة تعيين كلمة المرور، ثم انقر فوق **التكامل المحلي.**</span><span class="sxs-lookup"><span data-stu-id="e3e47-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="e3e47-117">هل تريد تعيين الخيار **"إعادة كتابة كلمات المرور"** إلى الدليل الخاص بك في الموقع؟ إلى **نعم.**</span><span class="sxs-lookup"><span data-stu-id="e3e47-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="e3e47-118">قم بتعيين الخيار السماح **للمستخدمين بإلغاء تأمين الحسابات دون إعادة تعيين كلمة المرور الخاصة بهم؟** إلى **نعم.**</span><span class="sxs-lookup"><span data-stu-id="e3e47-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="e3e47-119">عندما تكون جاهزا، انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="e3e47-119">When ready, click **Save**.</span></span>

<span data-ttu-id="e3e47-120">لمزيد من المعلومات، راجع تمكين إعادة تعيين كلمة مرور الخدمة الذاتية [ل Azure Active Directory إلى بيئة المحلية](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="e3e47-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="e3e47-121">عندما يقوم مسؤول بإعادة تعيين كلمة مرور مستخدم في مدخل Azure، إذا كان هذا المستخدم موحا أو متزامنا مع كلمة المرور، يتم إعادة كتابة كلمة المرور إلى الموقع.</span><span class="sxs-lookup"><span data-stu-id="e3e47-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="e3e47-122">تتطلب هذه الوظيفة ترخيص Azure Premium (P1 أو P2) وهو غير معتمد حاليا في مدخل مسؤول Office.</span><span class="sxs-lookup"><span data-stu-id="e3e47-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
