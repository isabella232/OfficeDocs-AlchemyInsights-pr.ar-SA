---
title: تمكين إعادة كتابة كلمة المرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: 1e90aedab20c8abaa021ed980e868cea0503b7b1
ms.sourcegitcommit: db95fd628c45d9810e5af5c5a4e6388c793339ac
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/03/2021
ms.locfileid: "50093342"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="222d0-102">تمكين إعادة كتابة كلمة المرور في Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="222d0-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="222d0-103">لتمكين إعادة تعيين الكتابة بكلمة مرور الخدمة الذاتية، قم أولا بتمكين خيار الكتابة في Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="222d0-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="222d0-104">من خادم Azure AD Connect، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="222d0-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="222d0-105">سجل الدخول إلى خادم Azure AD Connect وابدأ معالج تكوين **Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="222d0-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="222d0-106">على صفحة **الترحيب،** انقر فوق **"تكوين".**</span><span class="sxs-lookup"><span data-stu-id="222d0-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="222d0-107">في صفحة **المهام الإضافية،** حدد **"تخصيص خيارات المزامنة"،** ثم انقر فوق **"التالي".**</span><span class="sxs-lookup"><span data-stu-id="222d0-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="222d0-108">في صفحة **"الاتصال ب Azure AD"،** أدخل بيانات اعتماد المسؤول العام لمستأجر Azure، ثم انقر فوق **"التالي".**</span><span class="sxs-lookup"><span data-stu-id="222d0-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="222d0-109">في صفحات تصفية الدلائل **والمجال/OU** في Connect، انقر فوق **"التالي".** </span><span class="sxs-lookup"><span data-stu-id="222d0-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="222d0-110">في صفحة **الميزات الاختيارية،** حدد المربع بجانب إعادة كتابة كلمة **المرور** وانقر فوق **"التالي".**</span><span class="sxs-lookup"><span data-stu-id="222d0-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="222d0-111">في الصفحة **"جاهز لتكوين"،** انقر فوق **"تكوين"** وانتظر حتى تنتهي العملية.</span><span class="sxs-lookup"><span data-stu-id="222d0-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="222d0-112">عندما ترى انتهاء التكوين، انقر فوق **"إنهاء".**</span><span class="sxs-lookup"><span data-stu-id="222d0-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="222d0-113">مع تمكين إعادة كتابة كلمة المرور في Azure AD Connect، قم بتكوين Azure AD SSPR للكتابة.</span><span class="sxs-lookup"><span data-stu-id="222d0-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="222d0-114">لتمكين إعادة كتابة كلمة المرور في SSPR، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="222d0-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="222d0-115">سجل الدخول إلى مدخل Azure باستخدام حساب مسؤول عام.</span><span class="sxs-lookup"><span data-stu-id="222d0-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="222d0-116">ابحث عن **Azure Active Directory** وحدده، وانقر فوق إعادة **تعيين** كلمة المرور، ثم انقر **فوق التكامل المحلي.**</span><span class="sxs-lookup"><span data-stu-id="222d0-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="222d0-117">تعيين خيار إعادة كتابة كلمات المرور إلى الدليل **في الموقع؟** إلى **"نعم".**</span><span class="sxs-lookup"><span data-stu-id="222d0-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="222d0-118">تعيين الخيار "السماح للمستخدمين بإلغاء تأمين الحسابات دون إعادة تعيين كلمة المرور **الخاصة بهم"؟** إلى **"نعم".**</span><span class="sxs-lookup"><span data-stu-id="222d0-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="222d0-119">عندما تكون جاهزا، انقر فوق **"حفظ".**</span><span class="sxs-lookup"><span data-stu-id="222d0-119">When ready, click **Save**.</span></span>

<span data-ttu-id="222d0-120">لمزيد من المعلومات، راجع ["تمكين خدمة Azure Active Directory](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback)الذاتية" لإعادة تعيين إعادة الكتابة إلى بيئة المحلية.</span><span class="sxs-lookup"><span data-stu-id="222d0-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="222d0-121">عندما يعيد المسؤول تعيين كلمة مرور مستخدم في مدخل Azure، إذا كان هذا المستخدم موحنا أو متزامنا مع كلمة المرور، يتم إعادة كتابة كلمة المرور إلى الموقع</span><span class="sxs-lookup"><span data-stu-id="222d0-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="222d0-122">تتطلب هذه الوظيفة ترخيص Azure Premium (P1 أو P2) وهو غير معتمد حاليا في مدخل مسؤول Office.</span><span class="sxs-lookup"><span data-stu-id="222d0-122">This functionality requires Azure Premium License (P1 or P2) and is currently not supported in the Office Admin portal.</span></span>
