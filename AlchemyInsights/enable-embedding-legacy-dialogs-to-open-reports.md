---
title: تمكين تضمين الحوارات القديمة لفتح التقارير
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: ca0894849e95fd69acd2065c3f065547231a07f9
ms.sourcegitcommit: 0cf8d133d6feade6df8b1082444ce73faa91e145
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/13/2020
ms.locfileid: "44204647"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="ff37f-102">تمكين تضمين الحوارات القديمة لفتح التقارير</span><span class="sxs-lookup"><span data-stu-id="ff37f-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="ff37f-103">**اعراض**</span><span class="sxs-lookup"><span data-stu-id="ff37f-103">**Symptom**</span></span>

<span data-ttu-id="ff37f-104">يتعذر على المستخدمين فتح التقارير.</span><span class="sxs-lookup"><span data-stu-id="ff37f-104">Users are unable to open reports.</span></span> <span data-ttu-id="ff37f-105">"لقد حدث خطأ ما.</span><span class="sxs-lookup"><span data-stu-id="ff37f-105">"Something has gone wrong.</span></span> <span data-ttu-id="ff37f-106">تحقق من التفاصيل الفنية لمزيد من التفاصيل".</span><span class="sxs-lookup"><span data-stu-id="ff37f-106">Check technical details for more details."</span></span>

<span data-ttu-id="ff37f-107">**يسبب**</span><span class="sxs-lookup"><span data-stu-id="ff37f-107">**Cause**</span></span>

<span data-ttu-id="ff37f-108">تفشل التقارير في التحميل في UCI مع الخطأ، "واصف النموذج فارغة أو غير المعرفة."</span><span class="sxs-lookup"><span data-stu-id="ff37f-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="ff37f-109">لا تزال التقارير في UCI تتطلب حوارات قديمة، لذلك يحتاج نظام العميل إلى تمكين تمكين *التضمين القديم.*</span><span class="sxs-lookup"><span data-stu-id="ff37f-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="ff37f-110">**حل**</span><span class="sxs-lookup"><span data-stu-id="ff37f-110">**Solution**</span></span>

1. <span data-ttu-id="ff37f-111">انتقل إلى **إعدادات >إعدادات النظام > الإدارة > علامة التبويب العامة**.</span><span class="sxs-lookup"><span data-stu-id="ff37f-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="ff37f-112">تعيين "تمكين تضمين بعض الحوارات القديمة في عميل متصفح الواجهة الموحدة" إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="ff37f-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
