---
title: نشر تطبيق Intune Win32
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/06/2020
ms.locfileid: "48461725"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="aeb8d-102">نشر تطبيق Intune Win32</span><span class="sxs-lookup"><span data-stu-id="aeb8d-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="aeb8d-103">يسمح Microsoft Intune لتطبيقات Win32 ، بما في ذلك لكن لا تقتصر علي MSI و. سيتم نشره في الاجهزه التي تعمل بنظام Windows 10.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="aeb8d-104">تتطلب اليه النشر المستخدمة توفر ملحق الاداره ل Intune (IME) علي الجهاز الهدف.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="aeb8d-105">سيتم تثبيت محرر أسلوب الإدخال (IME) تلقائيا كنتيجة لاستهداف برنامج powershell نصي أو نشر تطبيق win32 إلى مستخدم/جهاز.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="aeb8d-106">هناك أيضا مجموعه من المتطلبات المسبقة التي يجب تحقيقها من أجل نشر تطبيقات Win32 التي تتضمن:</span><span class="sxs-lookup"><span data-stu-id="aeb8d-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="aeb8d-107">الانظمه الاساسيه المعتمدة: الإصدار 1607 أو الأحدث من Windows 10 (الإصدارات Enterprise و Pro والتعليمية).</span><span class="sxs-lookup"><span data-stu-id="aeb8d-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="aeb8d-108">البنية المعتمدة: x86 و x64.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="aeb8d-109">أداره الاجهزه: انضم إلى AAD وتم تسجيله تلقائيا (بما في ذلك المجال المختلط المرتبط بنهج المجموعة والتسجيل التلقائي).</span><span class="sxs-lookup"><span data-stu-id="aeb8d-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="aeb8d-110">تنسيق حزمه التطبيق:. **إينتونيوين**  الملفات التي تم تحضيرها بواسطة [أداه تحضير المحتوي Microsoft Win32](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span><span class="sxs-lookup"><span data-stu-id="aeb8d-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="aeb8d-111">تحديد</span><span class="sxs-lookup"><span data-stu-id="aeb8d-111">Limitations:</span></span>
    - <span data-ttu-id="aeb8d-112">الحد الأقصى للحجم: 8 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="aeb8d-113">الهندسة غير المعتمدة: الأذرع.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="aeb8d-114">راجع المستند "[أضافه تطبيق Win32 وتعيينه ومراقبته في Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" للحصول علي معلومات ذات صله بتلك الخطوات.</span><span class="sxs-lookup"><span data-stu-id="aeb8d-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="aeb8d-115">تفاصيل حول استكشاف أخطاء نشر التطبيقات علي Windows التي تتضمن تطبيقات Win32 يمكن مراجعتها في المستندات التالية</span><span class="sxs-lookup"><span data-stu-id="aeb8d-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="aeb8d-116">استكشاف مشاكل تثبيت التطبيق وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="aeb8d-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="aeb8d-117">استكشاف أخطاء تطبيقات Win32 وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="aeb8d-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)