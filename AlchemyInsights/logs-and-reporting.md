---
title: السجلات وإعداد التقارير
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/27/2021
ms.locfileid: "50035824"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="33794-102">السجلات وإعداد التقارير</span><span class="sxs-lookup"><span data-stu-id="33794-102">Logs and Reporting</span></span>

<span data-ttu-id="33794-103">تجيب الأسئلة الشائعة حول الأسئلة الشائعة حول إعداد تقارير Azure Active Directory (Azure AD) عن Azure Active [Directory.](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq)</span><span class="sxs-lookup"><span data-stu-id="33794-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="33794-104">لمزيد من المعلومات، راجع [إعداد تقارير Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="33794-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="33794-105">**استكشاف مشاكل التدقيق وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="33794-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="33794-106">إذا كنت تواجه مشاكل في رؤية بعض أنشطة [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)التدقيق وكان النشاط المفقود في هذه القائمة، فيرجى تقديم تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="33794-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="33794-107">إذا كنت تواجه مشاكل في رؤية أي سجلات تدقيق في المستأجر الخاص بك، فيرجى تقديم تذكرة دعم.</span><span class="sxs-lookup"><span data-stu-id="33794-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="33794-108">إذا لم تظهر أنشطة التدقيق الخاصة بك على الفور [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) في مدخل Azure، فافحص معلومات زمن الوصول لدينا وأدخل تذكرة دعم إذا تجاوز التأخير زمن الوصول الموثق.</span><span class="sxs-lookup"><span data-stu-id="33794-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="33794-109">استبقاء سجلات نشاط Azure AD</span><span class="sxs-lookup"><span data-stu-id="33794-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="33794-110">إذا لم تتمكن من رؤية كل التدقيق لنطاق التاريخ الذي حددته، يمكنك تنزيل ما يصل إلى 250 ألف صف (تم فرزها حسب أحدث) من تسجيلات الدخول من مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="33794-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="33794-111">لمزيد من المعلومات، راجع [تنزيل أنشطة التدقيق.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="33794-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="33794-112">**استكشاف مشاكل تسجيل الدخول وإصلاحها**</span><span class="sxs-lookup"><span data-stu-id="33794-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="33794-113">يمكنك فقط الاطلاع على آخر 30 يوما من البيانات إذا كان لديك ترخيص Azure AD Premium (P1 أو P2) للمستأجر الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="33794-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="33794-114">لا تتوفر تسجيلات الدخول إلا لمستأجري Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="33794-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="33794-115">وهو غير متوفر للمستأجرين المرخصين المجانيين أو الأساسيين.</span><span class="sxs-lookup"><span data-stu-id="33794-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="33794-116">إذا كان المستأجر لديك لديه ترخيص Premium P1 ولم تتمكن من رؤية [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) تسجيلات الدخول، فتحقق من معلومات زمن الوصول واحجز تذكرة دعم إذا تجاوز التأخير زمن الوصول الموثق.</span><span class="sxs-lookup"><span data-stu-id="33794-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="33794-117">إذا لم تتمكن من رؤية كل تسجيلات الدخول لنطاق التاريخ الذي حددته، لاحظ أنه يمكنك تنزيل ما يصل إلى 250 ألف صف (تم فرزها حسب أحدث) من تسجيلات الدخول من مدخل Azure.</span><span class="sxs-lookup"><span data-stu-id="33794-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="33794-118">لمزيد من المعلومات، راجع تنزيل أنشطة [تسجيل الدخول.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="33794-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="33794-119">**استكشاف مشاكل تقارير الأمان وإصلاحها (المستخدمون الذين تم وضع علامة "معرضون للمخاطر"، و"تسجيل الدخول المخطر")**</span><span class="sxs-lookup"><span data-stu-id="33794-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="33794-120">المستخدمون الذين تم وضع علامة "تقرير أمان المخاطر" لديهم</span><span class="sxs-lookup"><span data-stu-id="33794-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="33794-121">تقرير تسجيل الدخول المخطر في مدخل Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="33794-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="33794-122">أحداث مخاطر Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="33794-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
