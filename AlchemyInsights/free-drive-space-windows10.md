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
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034855"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="2f220-102">تحرير مساحة على محرك الأقراص في Windows 10</span><span class="sxs-lookup"><span data-stu-id="2f220-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="2f220-103">فيما يلي خياران لتحرير مساحة على محرك الأقراص في Windows:</span><span class="sxs-lookup"><span data-stu-id="2f220-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="2f220-104">حرر مساحة على محرك الأقراص في Windows 10.</span><span class="sxs-lookup"><span data-stu-id="2f220-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="2f220-105">حرر مساحة لتحديثات Windows 10 باستخدام جهاز تخزين خارجي.</span><span class="sxs-lookup"><span data-stu-id="2f220-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="2f220-106">إذا كان لا يزال لديك مساحة منخفضة على القرص بعد استخدام "تنظيف القرص"، فمن المحتمل أن مجلد Temp يمتلئ بسرعة بملفات التطبيق (appx.) المستخدمة بواسطة Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="2f220-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="2f220-107">لإصلاح هذه المشكلة، أعد تعيين المتجر، وأمسح ذاكرة التخزين المؤقت للمتجر، ثم قم بتشغيل مصلح مصلح Windows Update ومصلحها.</span><span class="sxs-lookup"><span data-stu-id="2f220-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="2f220-108">تأكد من إغلاق Microsoft Store قبل المتابعة إلى هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="2f220-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="2f220-109">**الخطوة 1: إعادة تعيين Microsoft Store**</span><span class="sxs-lookup"><span data-stu-id="2f220-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="2f220-110">**ملاحظة** ويحذف هذا بشكل دائم بيانات التطبيق على الجهاز، بما في ذلك تفضيلاتك وتفاصيل تسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="2f220-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="2f220-111">حدد **بدء**  >  **الإعدادات**  >  **تطبيقات التطبيقات**&  >  **الميزات**.</span><span class="sxs-lookup"><span data-stu-id="2f220-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="2f220-112">في قائمة التطبيقات، حدد موقع Microsoft Store وحدده.</span><span class="sxs-lookup"><span data-stu-id="2f220-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="2f220-113">حدد **خيارات متقدمة**.</span><span class="sxs-lookup"><span data-stu-id="2f220-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="2f220-114">قم بالتمرير لأسفل وحدد **إعادة تعيين**، ثم تأكيد **إعادة تعيين**.</span><span class="sxs-lookup"><span data-stu-id="2f220-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="2f220-115">**الخطوة 2: مسح ذاكرة التخزين المؤقت لمتجر Microsoft**</span><span class="sxs-lookup"><span data-stu-id="2f220-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="2f220-116">اضغط على مفتاح شعار Windows + R لفتح مربع الحوار تشغيل.</span><span class="sxs-lookup"><span data-stu-id="2f220-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="2f220-117">اكتب wsreset.exe وحدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="2f220-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="2f220-118">يتم فتح نافذة "موجه الأوامر" فارغة.</span><span class="sxs-lookup"><span data-stu-id="2f220-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="2f220-119">بعد حوالي 10 ثوان، يتم إغلاق النافذة ويفتح المتجر تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="2f220-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="2f220-120">**الخطوة 3: إعادة تعيين Windows Update**</span><span class="sxs-lookup"><span data-stu-id="2f220-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="2f220-121">حدد **بدء**  >  **الإعدادات**  >  **تحديث & استكشاف** الأخطاء  >  **وإصلاحها.**</span><span class="sxs-lookup"><span data-stu-id="2f220-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="2f220-122">قم بالتمرير لأسفل وحدد **Windows Update** من القائمة، وحدد تشغيل م استكشاف **المشاكل ومشكلاتها.**</span><span class="sxs-lookup"><span data-stu-id="2f220-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="2f220-123">إعادة تشغيل الكمبيوتر والتحقق مما إذا كنت لا تزال تواجه المشكلة.</span><span class="sxs-lookup"><span data-stu-id="2f220-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

