---
title: إضافة Microsoft Edge إلى Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/10/2021
ms.locfileid: "50194446"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="24f22-102">إضافة Microsoft Edge إلى Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="24f22-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="24f22-103">لكي تتمكن من نشر Microsoft Edge ل Windows 10 وتكوينه ومراقبته وحمايته، يجب أولا إضافته إلى Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="24f22-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="24f22-104">يدعم Intune Microsoft Edge 77 والإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="24f22-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="24f22-105">سيكتشف Intune أي عمليات تثبيت موجودة مسبقا ل Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="24f22-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="24f22-106">إذا كان Microsoft Edge مثبتا في سياق المستخدم، فإن تثبيت النظام سي الكتابة فوق التثبيت في سياق المستخدم.</span><span class="sxs-lookup"><span data-stu-id="24f22-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="24f22-107">إذا تم تثبيت Microsoft Edge في سياق النظام، سيتم إعلام نجاح التثبيت.</span><span class="sxs-lookup"><span data-stu-id="24f22-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="24f22-108">سيتم الكتابة فوق Microsoft Edge المثبت مسبقا والإصدارات الأحدث، لكل القنوات في سياق المستخدم، مع تثبيت Microsoft Edge في سياق النظام.</span><span class="sxs-lookup"><span data-stu-id="24f22-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="24f22-109">**المتطلبات الأساسية**</span><span class="sxs-lookup"><span data-stu-id="24f22-109">**Prerequisite**</span></span>

<span data-ttu-id="24f22-110">الإصدار 1709 من Windows 10 أو الإصدارات الأحدث</span><span class="sxs-lookup"><span data-stu-id="24f22-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="24f22-111">**خطوات إضافة Edge إلى Intune**</span><span class="sxs-lookup"><span data-stu-id="24f22-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="24f22-112">[تكوين التطبيق في Intune.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="24f22-113">[تكوين معلومات التطبيق.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="24f22-114">[تكوين إعدادات التطبيق.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="24f22-115">[حدد علامات النطاق (اختياري).](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="24f22-116">[أضف التطبيق.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="24f22-117">لمزيد من المساعدة، راجع [استكشاف الأخطاء وإصلاحها.](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge)</span><span class="sxs-lookup"><span data-stu-id="24f22-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




