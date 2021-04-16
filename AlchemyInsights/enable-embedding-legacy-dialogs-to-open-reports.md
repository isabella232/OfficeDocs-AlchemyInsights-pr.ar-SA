---
title: تفعيل تضمين مربعات الحوار القديمة لفتح التقارير
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
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814251"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="4d417-102">تفعيل تضمين مربعات الحوار القديمة لفتح التقارير</span><span class="sxs-lookup"><span data-stu-id="4d417-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="4d417-103">**العَرَض**</span><span class="sxs-lookup"><span data-stu-id="4d417-103">**Symptom**</span></span>

<span data-ttu-id="4d417-104">المستخدمون غير قادرين على فتح التقارير.</span><span class="sxs-lookup"><span data-stu-id="4d417-104">Users are unable to open reports.</span></span> <span data-ttu-id="4d417-105">"حدث خطأ ما.</span><span class="sxs-lookup"><span data-stu-id="4d417-105">"Something has gone wrong.</span></span> <span data-ttu-id="4d417-106">تحقق من التفاصيل الفنية لمزيد من التفاصيل ".</span><span class="sxs-lookup"><span data-stu-id="4d417-106">Check technical details for more details."</span></span>

<span data-ttu-id="4d417-107">**السبب**</span><span class="sxs-lookup"><span data-stu-id="4d417-107">**Cause**</span></span>

<span data-ttu-id="4d417-108">فشل تحميل التقارير في UCI مع ظهور الخطأ، "واصف النموذج فارغ أو غير محدد."</span><span class="sxs-lookup"><span data-stu-id="4d417-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="4d417-109">لا تزال التقارير في UCI تتطلب مربعات حوار قديمة، لذلك يحتاج نظام العميل إلى تمكين *allowlegacydialogsembedding*.</span><span class="sxs-lookup"><span data-stu-id="4d417-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="4d417-110">**الحل**</span><span class="sxs-lookup"><span data-stu-id="4d417-110">**Solution**</span></span>

1. <span data-ttu-id="4d417-111">انتقل إلى **الإعدادات > الإدارة > إعدادات النظام > علامة التبويب عام**.</span><span class="sxs-lookup"><span data-stu-id="4d417-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="4d417-112">قم بتعيين "تمكين تضمين بعض مربعات الحوار القديمة في عميل مستعرض "الواجهة الموحدة" على **نعم**.</span><span class="sxs-lookup"><span data-stu-id="4d417-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
