---
title: تمكين الكتابة الخلفية لكلمه المرور في Azure AD Connect
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
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560427"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="d8847-102">تمكين الكتابة الخلفية لكلمه المرور في Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="d8847-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="d8847-103">لتمكين أعاده تعيين كلمه مرور الخدمة الذاتية ، قم أولا بتمكين خيار الكتابة الخلفية في Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="d8847-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="d8847-104">من خادم Azure AD Connect ، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="d8847-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="d8847-105">سجل دخولك إلى خادم Azure AD Connect وأبدا بتشغيل معالج تكوين **AZURE Ad connect** .</span><span class="sxs-lookup"><span data-stu-id="d8847-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="d8847-106">علي صفحه **الترحيب** ، انقر فوق **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="d8847-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="d8847-107">في الصفحة **المهام الاضافيه** ، حدد **تخصيص خيارات المزامنة**، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="d8847-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="d8847-108">في صفحه **الاتصال ب AZURE AD** ، ادخل بيانات اعتماد المسؤول العمومي لمستاجر azure الخاص بك ، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="d8847-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="d8847-109">في الصفحتين **الاتصال بالدلائل** وتصفيه **المجال/الوحدة التنظيمية** ، انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="d8847-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="d8847-110">في صفحه **الميزات الاختيارية** ، حدد المربع إلى جانب **كتابه كلمه المرور** ، ثم انقر فوق **التالي**.</span><span class="sxs-lookup"><span data-stu-id="d8847-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="d8847-111">في الصفحة **جاهز للتكوين** ، انقر فوق **تكوين** وانتظر حتى تنتهي العملية.</span><span class="sxs-lookup"><span data-stu-id="d8847-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="d8847-112">عندما تري تاريخ انتهاء التكوين ، انقر فوق **إنهاء**.</span><span class="sxs-lookup"><span data-stu-id="d8847-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="d8847-113">باستخدام الكتابة الخلفية لكلمه المرور الممكنة في Azure AD Connect ، قم بتكوين Azure AD سبر للحصول علي الكتابة الخلفية</span><span class="sxs-lookup"><span data-stu-id="d8847-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="d8847-114">لتمكين الكتابة الخلفية لكلمه المرور في سبر ، أكمل الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="d8847-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="d8847-115">سجل دخولك إلى مدخل Azure باستخدام حساب مسؤول عام.</span><span class="sxs-lookup"><span data-stu-id="d8847-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="d8847-116">ابحث عن **Azure Active directory** وحدده ، وانقر فوق **أعاده تعيين كلمه المرور**، ثم انقر فوق **التكامل المحلي**.</span><span class="sxs-lookup"><span data-stu-id="d8847-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="d8847-117">تعيين خيار **كتابه كلمات المرور إلى الدليل المحلي ؟** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="d8847-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="d8847-118">تعيين الخيار الخاص **بتمكين المستخدمين من إلغاء تامين الحسابات من دون أعاده تعيين كلمه المرور الخاصة بهم ؟** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="d8847-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="d8847-119">عندما تكون جاهزا ، انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d8847-119">When ready, click **Save**.</span></span>

<span data-ttu-id="d8847-120">لمزيد من المعلومات ، راجع [تمكين أعاده تعيين كلمه مرور الخدمة الذاتية ل Azure active directory إلى بيئة محليه](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="d8847-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="d8847-121">عندما يقوم مسؤول باعاده تعيين كلمه مرور المستخدم في مدخل Azure ، إذا كان هذا المستخدم متزامنا أو تمت مزامنة تجزئه كلمه المرور ، ستتم كتابه كلمه المرور مره أخرى إلى محلي.</span><span class="sxs-lookup"><span data-stu-id="d8847-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="d8847-122">هذه الوظيفة غير معتمده حاليا في مدخل مسؤول Office.</span><span class="sxs-lookup"><span data-stu-id="d8847-122">This functionality is currently not supported in the Office Admin portal.</span></span>