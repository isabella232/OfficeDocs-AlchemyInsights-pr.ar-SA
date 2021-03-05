---
title: تكوين خدمة توفير الخدمة
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480961"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="8fa3a-102">تكوين خدمة توفير الخدمة</span><span class="sxs-lookup"><span data-stu-id="8fa3a-102">Configuring the Provision service</span></span>

<span data-ttu-id="8fa3a-103">لكي يعمل توفير خدمة المستخدم التلقائي، يتطلب Azure AD بيانات اعتماد صالحة تسمح له بالاتصال ب API الخاصة ب Workday Web Services.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="8fa3a-104">علاوة على ذلك، فإن الزر "اختبار الاتصال" في تطبيق توفير يوم العمل بمستخدم AD يقوم أيضا بالتحقق من صحة ما إذا كان قادرا على الاتصال بعامل توفير Azure AD Connect المقترن بمجال AD.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="8fa3a-105">إذا كان مدخل Azure قد أرجع خطأ عند حفظ بيانات الاعتماد، فاتبع الخطوات الموصى بها أدناه:</span><span class="sxs-lookup"><span data-stu-id="8fa3a-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="8fa3a-106">تأكد من تكوين حساب مستخدم نظام تكامل Workday كما هو م ذكر في قسم البرنامج التعليمي تكوين مستخدم نظام التكامل [في Workday.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)</span><span class="sxs-lookup"><span data-stu-id="8fa3a-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="8fa3a-107">تأكد من أن خدمة عامل توفير خدمة توفير خدمة Azure AD Connect قيد التشغيل على خادم Windows المحلي باستخدام وحدة تحكم إدارة الخدمات.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="8fa3a-108">يمكنك أيضا التحقق من حالة الوكيل في مدخل Azure بالنقر فوق الزر "عرض الوكيل المحلي".</span><span class="sxs-lookup"><span data-stu-id="8fa3a-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="8fa3a-109">تأكد من إدخال قيمة حقل "اسم مستخدم يوم العمل" باستخدام التنسيق username@workday المستأجر-المستأجر.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="8fa3a-110">إذا كان اسم يوم العمل-المستأجر مفقودا، تفشل مصادقة يوم العمل.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="8fa3a-111">إذا كنت تقوم بتكوين التكامل مع مستأجر تنفيذ يوم العمل، فلاحظ ساعات التوقف المجدولة لمستأجر يوم العمل.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="8fa3a-112">لقد حدد يوم العمل وقت التنفيذ المجدول لمستأجري التنفيذ خلال عطلات نهاية الأسبوع (عادة من مساء الجمعة إلى صباح السبت) كما أن حالات فشل الاتصال أثناء نافذة وقت التوقف هي مشكلة معروفة يتم حلها بشكل تلقائي بمجرد عودة مستأجري التنفيذ إلى وضع الاتصال.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="8fa3a-113">في حالات نادرة، قد ترى هذا الخطأ أيضا إذا تغيرت كلمة مرور مستخدم نظام التكامل بسبب تحديث المستأجر أو إذا كان الحساب في حالة مقفلة أو منتهية الصلاحية.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="8fa3a-114">يرجى التحقق من حالة مستخدم "نظام التكامل" مع مسؤول يوم العمل.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="8fa3a-115">لمزيد من التفاصيل حول تكوين يوم العمل للتكوين التلقائي، راجع البرنامج [التعليمي: تكوين يوم](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)عمل للتكوين التلقائي للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="8fa3a-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
