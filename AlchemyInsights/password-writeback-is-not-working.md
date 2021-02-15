---
title: لا يعمل "كتابة كلمة المرور"
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243217"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="3aa69-102">لا يعمل "كتابة كلمة المرور"</span><span class="sxs-lookup"><span data-stu-id="3aa69-102">Password Writeback is not working</span></span>

<span data-ttu-id="3aa69-103">**أواجه مشاكل في تكوين إعادة كتابة كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="3aa69-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="3aa69-104">الكتابة بكلمة مرور هي ميزة متميزة.</span><span class="sxs-lookup"><span data-stu-id="3aa69-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="3aa69-105">تأكد من فهم متطلبات الترخيص:</span><span class="sxs-lookup"><span data-stu-id="3aa69-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="3aa69-106">يجب أن يكون لديك ترخيص واحد على الأقل تم تعيينه في مؤسستك</span><span class="sxs-lookup"><span data-stu-id="3aa69-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="3aa69-107">**مستخدمو السحابة فقط** - أي SKU مدفوعة من Office 365 (O365) أو Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="3aa69-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="3aa69-108">المستخدمون في السحابة **و/أو** المحليون - Azure AD Premium P1 أو P2 أو Enterprise Mobility + Security (EMS) أو Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="3aa69-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="3aa69-109">لمعرفة المزيد حول متطلبات الترخيص، راجع متطلبات الترخيص لإعادة تعيين كلمة مرور الخدمة الذاتية ل [Azure AD](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="3aa69-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="3aa69-110">لديك حساب مسؤول واحد على الأقل، حساب مستخدم اختباري واحد مع أحد الترخيص المناسب.</span><span class="sxs-lookup"><span data-stu-id="3aa69-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="3aa69-111">يجب توصيل Azure AD Connect ب "محاكي وحدة تحكم المجال الأساسية" لكي تعمل كتابة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="3aa69-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="3aa69-112">يمكنك تكوين Azure AD Connect لاستخدام وحدة التحكم بالمجال  الأساسي بالنقر ب الماوس الأيمن فوق خصائص موصل مزامنة Active Directory، ثم تحديد أقسام تكوين **الدليل.**</span><span class="sxs-lookup"><span data-stu-id="3aa69-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="3aa69-113">من هناك، ابحث  عن مقطع إعدادات اتصال وحدة التحكم بالمجال ودقق في المربع بعنوان استخدام وحدات تحكم المجال **المفضلة فقط.**</span><span class="sxs-lookup"><span data-stu-id="3aa69-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="3aa69-114">إذا لم تكن DC المفضلة محاكاة PDC، فإن Azure AD Connect سيبقى يصل إلى PDC لكتابة كلمة المرور.</span><span class="sxs-lookup"><span data-stu-id="3aa69-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="3aa69-115">تم تكوين إعادة تعيين كلمة المرور وتمكينها في المستأجر.</span><span class="sxs-lookup"><span data-stu-id="3aa69-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="3aa69-116">لمزيد من المعلومات، راجع ["تمكين المستخدمين" من إعادة تعيين كلمات مرور Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="3aa69-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="3aa69-117">تأكد من أن حساب المسؤول الذي يتم استخدامه لتمكين "كتابة كلمة المرور" هو حساب مسؤول مجموعة النظراء (تم إنشاؤه في Azure AD وليس AD المحلي)</span><span class="sxs-lookup"><span data-stu-id="3aa69-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="3aa69-118">لديك نشر AD واحد أو متعدد الغابات في موقع ويب يعمل بنظام التشغيل Windows Server 2008 R2 أو Windows Server 2012 أو Windows Server 2012 R2 مع تثبيت أحدث حزم الخدمات</span><span class="sxs-lookup"><span data-stu-id="3aa69-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="3aa69-119">لديك أداة Azure AD Connect مثبتة وقد أعددت بيئة AD للمزامنة إلى السحابة.</span><span class="sxs-lookup"><span data-stu-id="3aa69-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="3aa69-120">قبل اختبار إعادة كتابة كلمة المرور، تأكد من إكمال عملية الاستيراد والمزامنة الكاملة أولا من كل من AD و Azure AD في Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="3aa69-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="3aa69-121">لمعرفة المزيد، راجع كيفية القيام بمزامنة [واستيراد كامل في Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="3aa69-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="3aa69-122">**أواجه مشكلة في اتصال إعادة كتابة كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="3aa69-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="3aa69-123">تنزيل أحدث إصدار من [Azure AD Connect وتمكينه](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="3aa69-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="3aa69-124">تكوين جدار الحماية: ستحتاج أداة Azure AD Connect (1.1.443 والأعلى) إلى الوصول الصادر **إلى HTTPS:**</span><span class="sxs-lookup"><span data-stu-id="3aa69-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="3aa69-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3aa69-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="3aa69-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="3aa69-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="3aa69-127">السماح لاتصالات الخمول أن تستمر لمدة 2-3 دقائق على الأقل</span><span class="sxs-lookup"><span data-stu-id="3aa69-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="3aa69-128">**ما زلت أواجه مشاكل في إعادة كتابة كلمة المرور**</span><span class="sxs-lookup"><span data-stu-id="3aa69-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="3aa69-129">إذا كنت لا تزال تواجه صعوبة، فحاول تعطيل خدمة إعادة كتابة كلمة المرور في أداة Azure AD Connect ثم إعادة تمكينها</span><span class="sxs-lookup"><span data-stu-id="3aa69-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="3aa69-130">لمعرفة المزيد، راجع كيفية [تعطيل إعادة تمكين إعادة كتابة كلمة المرور](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="3aa69-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
