---
title: تكوين خدمة مزامنة MIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480838"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="c507b-102">تكوين خدمة مزامنة MIM</span><span class="sxs-lookup"><span data-stu-id="c507b-102">Configure MIM Sync service</span></span>

<span data-ttu-id="c507b-103">إن خدمة مزامنة Microsoft Identity Manager (MIM) هي أحد مكونات MIM.</span><span class="sxs-lookup"><span data-stu-id="c507b-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="c507b-104">إنها خدمة مركزية في الموقع المحلية تخزن المعلومات وتكاملها مع المؤسسات التي لديها العديد من الدلائل وقواعد البيانات المحلية.</span><span class="sxs-lookup"><span data-stu-id="c507b-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="c507b-105">قد تتمكن من حل مشكلتك في "مزامنة MIM" إذا تم حل المشكلة في تحديث حديث ل MIM أو إذا كانت إحدى المشاكل الأخرى المذكورة في القسم أدناه.</span><span class="sxs-lookup"><span data-stu-id="c507b-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="c507b-106">**الخطوات المستحسنة**</span><span class="sxs-lookup"><span data-stu-id="c507b-106">**Recommended steps**</span></span>

1. <span data-ttu-id="c507b-107">تأكد من أنك تستخدم تحديثا حديثا لمزامنة MIM وتحقق من ملاحظات إصدار [مزامنة MIM](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) لتحديد ما إذا تم حل المشكلة في تحديث.</span><span class="sxs-lookup"><span data-stu-id="c507b-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="c507b-108">إذا كانت المشكلة في موصل GENERIC LDAP أو SQL العام أو Lotus Domino أو Web Services، فتأكد من أنك تستخدم تحديثا حديثا [للموصلات العامة.](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)</span><span class="sxs-lookup"><span data-stu-id="c507b-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="c507b-109">إذا توقف تشغيل مزامنة MIM مع وجود [](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) خطأ، فاستشارة جدول رموز خطأ التشغيل لتحديد الأسباب المحتملة.</span><span class="sxs-lookup"><span data-stu-id="c507b-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="c507b-110">إذا توقف التشغيل مع استثناء ملحق **dll،** انقر فوق  هذه الكلمات لفتح نافذة خصائص "كائن المسافة للموصل"، وانقر فوق "تتبع المكدس"... للاطلاع على مزيد من المعلومات حول السبب الأساسي، كما هو موضح في [Extension-DLL-Exception.](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) </span><span class="sxs-lookup"><span data-stu-id="c507b-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="c507b-111">إذا كان مكون خدمة الإعلام بتغيير كلمة المرور (PCNS) يظهر الخطأ **6025** في سجل الأحداث أثناء مزامنة كلمة المرور، فتحقق من دليل استكشاف أخطاء إرسال تقرير PCNS وإصلاحها [6025.](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)</span><span class="sxs-lookup"><span data-stu-id="c507b-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="c507b-112">إذا كانت المزامنة الكاملة مع عامل إدارة خدمات  FIM بطيئة، فتحقق من إعداد النمو التلقائي ل TempDB، كما هو موضح في استكشاف الأخطاء وإصلاحها بالمزامنة الكاملة البطيئة أو [المعلقة.](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)</span><span class="sxs-lookup"><span data-stu-id="c507b-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="c507b-113">إذا كنت تواجه خطأ خادم متوقف مع خدمات فشل الإنشاء عبر الويب باستخدام عامل إدارة خدمات FIM، فشاهد ["معلومات الدعم": فشل إنشاء-عبر-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) للحصول على نظرة عامة حول الأسباب.</span><span class="sxs-lookup"><span data-stu-id="c507b-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

