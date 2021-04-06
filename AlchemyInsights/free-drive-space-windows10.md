---
title: تحرير مساحة على محرك الأقراص في Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505343"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="5a765-102">تحرير مساحة على محرك الأقراص في Windows 10</span><span class="sxs-lookup"><span data-stu-id="5a765-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="5a765-103">إليك خياران لتحرير مساحة على محرك الأقراص في Windows:</span><span class="sxs-lookup"><span data-stu-id="5a765-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="5a765-104">تحرير مساحة على محرك الأقراص في Windows 10.</span><span class="sxs-lookup"><span data-stu-id="5a765-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="5a765-105">قم بتحرير مساحة لتحديثات Windows 10 باستخدام جهاز تخزين خارجي.</span><span class="sxs-lookup"><span data-stu-id="5a765-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="5a765-106">إذا كنت لا تزال تعاني من انخفاض مساحة القرص بعد استخدام أداة تنظيف القرص، فمن الممكن أن يمتلئ المجلد المؤقت بسرعة بملفات التطبيقات (appx.) التي يستخدمها Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="5a765-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="5a765-107">لإصلاح هذه المشكلة، قم بإعادة تعيين Microsoft Store، وامسح ذاكرة التخزين المؤقت، ثم قم بتشغيل مستكشف أخطاء Windows Update ومصلحها.</span><span class="sxs-lookup"><span data-stu-id="5a765-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="5a765-108">تأكد من إغلاق Microsoft Store قبل متابعة هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="5a765-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="5a765-109">**الخطوة 1: إعادة تعيين Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="5a765-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="5a765-110">**ملاحظة** يؤدي هذا إلى حذف بيانات التطبيق بشكل دائم على الجهاز، بما في ذلك تفضيلاتك وتفاصيل تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="5a765-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="5a765-111">حدد **بدء** > **الإعدادات** > **التطبيقات** > **التطبيقات والميزات**.</span><span class="sxs-lookup"><span data-stu-id="5a765-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="5a765-112">في قائمة التطبيقات، ابحث عن Microsoft Store وحدده.</span><span class="sxs-lookup"><span data-stu-id="5a765-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="5a765-113">حدد **خيارات متقدمة**.</span><span class="sxs-lookup"><span data-stu-id="5a765-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="5a765-114">قم بالتمرير لأسفل وحدد **إعادة تعيين**، ثم **تأكيد إعادة التعيين**.</span><span class="sxs-lookup"><span data-stu-id="5a765-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="5a765-115">**الخطوة 2: مسح ذاكرة التخزين المؤقت في Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="5a765-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="5a765-116">اضغط على مفتاح شعار Windows + R لفتح مربع الحوار "تشغيل".</span><span class="sxs-lookup"><span data-stu-id="5a765-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="5a765-117">اكتب "wsreset.exe" وحدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="5a765-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="5a765-118">ستُفتح نافذة موجه أوامر فارغة.</span><span class="sxs-lookup"><span data-stu-id="5a765-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="5a765-119">بعد حوالي 10 ثوانٍ، تُغلق النافذة ويفتح Microsoft Store تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="5a765-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="5a765-120">**الخطوة 3: إعادة تعيين Windows Update**</span><span class="sxs-lookup"><span data-stu-id="5a765-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="5a765-121">حدد **بدء** > **الإعدادات** > **التحديث والأمان** > **استكشاف الأخطاء وإصلاحها**.</span><span class="sxs-lookup"><span data-stu-id="5a765-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="5a765-122">قم بالتمرير لأسفل وحدد **Windows Update** من القائمة، وحدد **تشغيل مستكشف الأخطاء ومصلحها**.</span><span class="sxs-lookup"><span data-stu-id="5a765-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="5a765-123">أعد تشغيل الكمبيوتر وتحقق مما إذا كنت لا تزال تواجه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="5a765-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

