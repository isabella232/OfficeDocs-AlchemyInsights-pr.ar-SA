---
title: استكشاف مشاكل تثبيت MDATP وإصلاحها على جهاز Mac
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743137"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a><span data-ttu-id="c452a-102">استكشاف مشاكل تثبيت MDATP وإصلاحها على جهاز Mac</span><span class="sxs-lookup"><span data-stu-id="c452a-102">Troubleshoot MDATP installation problems on a Mac</span></span>

<span data-ttu-id="c452a-103">إذا فشل التثبيت اليدوي، تظهر صفحة **الملخص** لمعالج التثبيت الخطأ التالي:</span><span class="sxs-lookup"><span data-stu-id="c452a-103">If manual installation fails, the **Summary** page of the installation wizard shows the following error:</span></span>

<span data-ttu-id="c452a-104">"حدث خطأ أثناء التثبيت.</span><span class="sxs-lookup"><span data-stu-id="c452a-104">"An error occurred during installation.</span></span> <span data-ttu-id="c452a-105">واجه المثبت خطأ تسبب في فشل التثبيت.</span><span class="sxs-lookup"><span data-stu-id="c452a-105">The Installer encountered an error that caused the installation to fail.</span></span> <span data-ttu-id="c452a-106">اتصل بالشركة المصنعة للبرامج للحصول على المساعدة."</span><span class="sxs-lookup"><span data-stu-id="c452a-106">Contact the software manufacturer for assistance."</span></span>

<span data-ttu-id="c452a-107">بالنسبة إلى عمليات نشر MDM، تظهر الصفحة فشلا عاما في التثبيت أيضا.</span><span class="sxs-lookup"><span data-stu-id="c452a-107">For MDM deployments, the page shows a generic installation failure, too.</span></span>

<span data-ttu-id="c452a-108">على الرغم من أننا لا نعرض أخطاء دقيقة للمستخدمين النهائيين، إلا أننا نحتفظ بملف سجل مع تقدم التثبيت، في **/Library/Logs/Microsoft/mdatp/install.log**.</span><span class="sxs-lookup"><span data-stu-id="c452a-108">Although we don't display exact errors to end users, we keep a log file with installation progress, in **/Library/Logs/Microsoft/mdatp/install.log**.</span></span> <span data-ttu-id="c452a-109">يتم إلحاق كل جلسة عمل تثبيت إلى ملف السجل هذا.</span><span class="sxs-lookup"><span data-stu-id="c452a-109">Each installation session appends to this log file.</span></span> <span data-ttu-id="c452a-110">لاخراج جلسة التثبيت الأخيرة فقط، استخدم `sed` .</span><span class="sxs-lookup"><span data-stu-id="c452a-110">To output the last installation session only, use `sed`.</span></span>

<span data-ttu-id="c452a-111">لمعرفة المزيد، راجع استكشاف مشاكل التثبيت وإصلاحها [ل Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span><span class="sxs-lookup"><span data-stu-id="c452a-111">To learn more, see [Troubleshoot installation issues for Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).</span></span>
