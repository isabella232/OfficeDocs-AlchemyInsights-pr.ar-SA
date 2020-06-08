---
title: تمكين رد كتابة كلمة المرور في Azure AD Connect
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002933"
- "5615"
ms.openlocfilehash: ab4b8692799d08363e1d726f72a3b80dcb598797
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204612"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="9b2c4-102">تمكين رد كتابة كلمة المرور في Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="9b2c4-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="9b2c4-103">لتمكين إعادة تعيين كلمة مرور الخدمة الذاتية، قم أولاً بتمكين خيار إعادة الكتابة في Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="9b2c4-104">من خادم Azure AD Connect، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9b2c4-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="9b2c4-105">قم بتسجيل الدخول إلى خادم Azure AD Connect وبدء تشغيل معالج تكوين **Azure AD Connect.**</span><span class="sxs-lookup"><span data-stu-id="9b2c4-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="9b2c4-106">في صفحة **الترحيب،** انقر فوق **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="9b2c4-107">في صفحة **المهام الإضافية،** حدد **تخصيص خيارات المزامنة،** ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="9b2c4-108">في صفحة **"الاتصال بـ Azure AD"،** أدخل بيانات اعتماد مسؤول عمومية لمستأجر Azure، ثم انقر فوق التالي.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click Next.</span></span>
5. <span data-ttu-id="9b2c4-109">في **الدلائل الاتصال** وصفحات تصفية **المجال / OU،** انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="9b2c4-110">في صفحة **الميزات الاختيارية،** حدد المربع المجاور **لاستعادة كلمة المرور** وانقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="9b2c4-111">في الصفحة **الجاهزة لتكوين،** انقر فوق **تكوين** وانتظر حتى تنتهي العملية.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="9b2c4-112">عندما ترى الانتهاء من التكوين، انقر فوق **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="9b2c4-113">مع تمكين إعادة كتابة كلمة المرور في Azure AD Connect ، قم الآن بتكوين Azure AD SSPR لإعادة الكتابة.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-113">With password writeback enabled in Azure AD Connect, now configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="9b2c4-114">لتمكين إعادة كتابة كلمة المرور في SSPR، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9b2c4-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="9b2c4-115">تسجيل الدخول إلى بوابة Azure باستخدام حساب مسؤول عمومي.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="9b2c4-116">البحث عن الدليل **النشط Azure**وتحديده ، انقر فوق إعادة تعيين **كلمة المرور**، ثم اختر التكامل **الداخلي**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-116">Search for and select **Azure Active Directory**, click **Password reset**, then choose **On-premises integration**.</span></span>
3. <span data-ttu-id="9b2c4-117">تعيين خيار **إعادة كتابة كلمات المرور إلى الدليل الداخلي الخاص بك؟** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="9b2c4-118">تعيين خيار **السماح للمستخدمين بإلغاء تأمين الحسابات دون إعادة تعيين كلمة المرور الخاصة بهم؟** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="9b2c4-119">عندما تكون جاهزة، انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="9b2c4-119">When ready, click **Save**.</span></span>

<span data-ttu-id="9b2c4-120">لمزيد من المعلومات، راجع [تمكين كلمة مرور الخدمة الذاتية للدليل النشط Azure إعادة تعيين الكتابة إلى بيئة داخلية](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="9b2c4-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>
