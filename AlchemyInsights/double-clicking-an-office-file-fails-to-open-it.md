---
title: فشل النقر نقرا مزدوجا فوق أحد ملفات Office لفتحه
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: 9dc4196cd36c8682e4d047e8abad493be97ced3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812066"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="efb3d-102">فشل النقر نقرا مزدوجا فوق أحد ملفات Office لفتحه</span><span class="sxs-lookup"><span data-stu-id="efb3d-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="efb3d-103">بعد النقر نقرا مزدوجا فوق ملف Office ، قد يظهر البرنامج مفتوحا ولكن لا يتم فتح الملف نفسه.</span><span class="sxs-lookup"><span data-stu-id="efb3d-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="efb3d-104">أو قد تتلقي رسالة الخطا: "حدثت مشكله اثناء إرسال الأمر إلى البرنامج."</span><span class="sxs-lookup"><span data-stu-id="efb3d-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="efb3d-105">هناك العديد من الأسباب المحتملة ، ولكن الحلان الأكثر شيوعا هما:</span><span class="sxs-lookup"><span data-stu-id="efb3d-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="efb3d-106">من داخل Excel ، تاكد من إلغاء تحديد الخيار DDE.</span><span class="sxs-lookup"><span data-stu-id="efb3d-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="efb3d-107">يمكن العثور علي الخيار بإنشاء مصنف جديد ثم اختيار **خيارات > الملفات > متقدمة**.</span><span class="sxs-lookup"><span data-stu-id="efb3d-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="efb3d-108">في المقطع **عام** ، قم بإلغاء تحديد الاختيار **تجاهل التطبيقات الأخرى التي تستخدم تبادل البيانات الديناميكي (DDE)**.</span><span class="sxs-lookup"><span data-stu-id="efb3d-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="efb3d-109">قم بتشغيل "إصلاح عبر الإنترنت" لاستعاده الإعدادات الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="efb3d-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="efb3d-110">انقر فوق زر بدء Windows وابحث عن "لوحه التحكم".</span><span class="sxs-lookup"><span data-stu-id="efb3d-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="efb3d-111">افتح **لوحه التحكم**، وانتقل إلى **البرامج > البرامج والميزات**.</span><span class="sxs-lookup"><span data-stu-id="efb3d-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="efb3d-112">ثم انقر بزر الماوس الأيمن فوق **Microsoft Office [الإصدار]** ثم اختر **تغيير > إصلاح عبر الإنترنت**.</span><span class="sxs-lookup"><span data-stu-id="efb3d-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="efb3d-113">إذا لم ينجح اي من هذه الحلول ، فيمكن العثور علي قائمه كامله بالحلول في مقاله الدعم ، [والنقر نقرا مزدوجا فوق ملف Office يفشل في فتحه](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span><span class="sxs-lookup"><span data-stu-id="efb3d-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
