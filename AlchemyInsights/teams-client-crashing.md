---
title: هل يتوقف عميل Teams عن العمل؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: ce37b260d126f876d2b6177515bd8a7c3874ef2c
ms.sourcegitcommit: d02e2b73aa7d0453d7baca1ea5a186cf6081d022
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2020
ms.locfileid: "43030498"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="940e3-102">هل يتوقف عميل Teams عن العمل؟</span><span class="sxs-lookup"><span data-stu-id="940e3-102">Teams client crashing?</span></span>

<span data-ttu-id="940e3-103">إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="940e3-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="940e3-104">إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="940e3-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="940e3-105">تأكد من توفر إمكانية الوصول إلى جميع [نطاقات URL الخاصة بـ Office 365 وعناوينه](https://docs.microsoft.com/microsoftteams/connectivity-issues).</span><span class="sxs-lookup"><span data-stu-id="940e3-105">Make sure all the [Office 365 URL's and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="940e3-106">سجّل الدخول باستخدام حساب المسؤول الخاص بك وتحقق من[لوحة معلومات حالة الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود انقطاع بالخدمة أو عدم تدنيها.</span><span class="sxs-lookup"><span data-stu-id="940e3-106">Log in with your admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

 - <span data-ttu-id="940e3-107">تكمن الخطوة الأخيرة في أن تحاول مسح ذاكرة التخزين المؤقت لعميل Teams لديك:</span><span class="sxs-lookup"><span data-stu-id="940e3-107">As a last step, you can attempt to clear your Teams client cache:</span></span>

    1.  <span data-ttu-id="940e3-108">قم بالخروج من عميل تطبيق سطح المكتب من Microsoft Teams بشكل كامل.</span><span class="sxs-lookup"><span data-stu-id="940e3-108">Fully exit the Microsoft Teams desktop client.</span></span> <span data-ttu-id="940e3-109">انقر بزر الماوس الأيمن فوق **Teams** من مقطع شريط مهام الأيقونات وانقر فوق **إنهاء** أو قم بتشغيل إدارة المهام وقم بإنهاء العملية بالكامل.</span><span class="sxs-lookup"><span data-stu-id="940e3-109">You can right-click **Teams** from the Icon Tray and click **Quit**, or run Task Manager and fully kill the process.</span></span>

    2.  <span data-ttu-id="940e3-110">انتقل إلى مستكشف الملفات واكتب %appdata%\Microsoft\teams.</span><span class="sxs-lookup"><span data-stu-id="940e3-110">Go to File Explorer, and type in %appdata%\Microsoft\teams.</span></span>

    3.  <span data-ttu-id="940e3-111">بعد الانتقال، سترى بعض الملفات التالية:</span><span class="sxs-lookup"><span data-stu-id="940e3-111">Once in the directory, you'll see a few of the following folders:</span></span>

         - <span data-ttu-id="940e3-112">من داخل **ذاكرة التخزين المؤقت للتطبيق**، انتقل إلى ذاكرة التخزين المؤقت واحذف أي ملفات موجودة في موقع ذاكرة التخزين المؤقت:  %appdata%\Microsoft\teams\application cache\cache.</span><span class="sxs-lookup"><span data-stu-id="940e3-112">From within **Application Cache**, go to Cache and delete any of the files in the Cache location:  %appdata%\Microsoft\teams\application cache\cache.</span></span>

        - <span data-ttu-id="940e3-113">من داخل **Blob_storage**، احذف كل الملفات: %appdata%\Microsoft\teams\blob_storage.</span><span class="sxs-lookup"><span data-stu-id="940e3-113">From within **Blob_storage**, delete all files: %appdata%\Microsoft\teams\blob_storage.</span></span>

        - <span data-ttu-id="940e3-114">من داخل **ذاكرة التخزين المؤقت**، احذف الملفات: %appdata%\Microsoft\teams\Cache.</span><span class="sxs-lookup"><span data-stu-id="940e3-114">From within **Cache**, delete all files: %appdata%\Microsoft\teams\Cache.</span></span>

        - <span data-ttu-id="940e3-115">من داخل **قواعد البيانات**، احذف كل الملفات: %appdata%\Microsoft\teams\databases.</span><span class="sxs-lookup"><span data-stu-id="940e3-115">From within **databases**, delete all files: %appdata%\Microsoft\teams\databases.</span></span>

        - <span data-ttu-id="940e3-116">من داخل **GPUCache**، احذف كل الملفات: %appdata%\Microsoft\teams\GPUcache.</span><span class="sxs-lookup"><span data-stu-id="940e3-116">From within **GPUCache**, delete all files: %appdata%\Microsoft\teams\GPUcache.</span></span>

        - <span data-ttu-id="940e3-117">من داخل **IndexedDB**، احذف ملف .db file: %appdata%\Microsoft\teams\IndexedDB.</span><span class="sxs-lookup"><span data-stu-id="940e3-117">From within **IndexedDB**, delete the .db file: %appdata%\Microsoft\teams\IndexedDB.</span></span>

        - <span data-ttu-id="940e3-118">من داخل **سعة التخزين المحلية**، احذف كل الملفات: %appdata%\Microsoft\teams\Local Storage.</span><span class="sxs-lookup"><span data-stu-id="940e3-118">From within **Local Storage**, delete all files: %appdata%\Microsoft\teams\Local Storage.</span></span>

        - <span data-ttu-id="940e3-119">وأخيراً، من داخل **tmp**، احذف أي ملف: %appdata%\Microsoft\teams\tmp.</span><span class="sxs-lookup"><span data-stu-id="940e3-119">Lastly, from within **tmp**, delete any file: %appdata%\Microsoft\teams\tmp.</span></span>

    4. <span data-ttu-id="940e3-120">إعادة تشغيل عميل Teams لديك.</span><span class="sxs-lookup"><span data-stu-id="940e3-120">Restart your Teams client.</span></span>
