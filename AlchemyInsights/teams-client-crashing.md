---
title: هل يتوقف عميل Teams عن العمل؟
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002323"
- "4512"
ms.openlocfilehash: 39310233eae83ceb18c6ff82451ae747f3c50048
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47691094"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="5cfd9-102">هل يتوقف عميل Teams عن العمل؟</span><span class="sxs-lookup"><span data-stu-id="5cfd9-102">Teams client crashing?</span></span>

<span data-ttu-id="5cfd9-103">إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="5cfd9-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="5cfd9-104">إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="5cfd9-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="5cfd9-105">تاكد من امكانيه الوصول إلى كل [عناوين url ونطاقات عناوين Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) .</span><span class="sxs-lookup"><span data-stu-id="5cfd9-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="5cfd9-106">سجل الدخول باستخدام حساب مسؤول المستاجر الخاص بك ، وتحقق من [لوحه معلومات حماية الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود اي انقطاع أو انخفاض في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="5cfd9-107">إلغاء تثبيت تطبيق الفرق وأعاده تثبيته (ارتباط)</span><span class="sxs-lookup"><span data-stu-id="5cfd9-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="5cfd9-108">استعرض وصولا إلى المجلد%appdata%\Microsoft\teams\ علي الكمبيوتر واحذف كل الملفات في هذا الدليل.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="5cfd9-109">قم [بتنزيل تطبيق الفرق وتثبيته](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)، ويمكنك تثبيت الفرق كمسؤول (بالنقر بزر الماوس الأيمن فوق مثبت الفرق وتحديد "تشغيل كمسؤول" في حال توفره).</span><span class="sxs-lookup"><span data-stu-id="5cfd9-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="5cfd9-110">إذا ما زال عميل الفرق معطلا ، فهل يمكنك أعاده إنتاج المشكلة ؟</span><span class="sxs-lookup"><span data-stu-id="5cfd9-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="5cfd9-111">إذا كان الأمر كذلك:</span><span class="sxs-lookup"><span data-stu-id="5cfd9-111">If so:</span></span>

1. <span data-ttu-id="5cfd9-112">استخدم مسجل الخطوات لتسجيل الخطوات.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="5cfd9-113">اغلق جميع التطبيقات غير الضرورية أو السرية.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="5cfd9-114">أبدا تشغيل مسجل الخطوات واعد إنشاء المشكلة اثناء تسجيل الدخول باستخدام حساب المستخدم المتاثر.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="5cfd9-115">[جمع سجلات الفرق التي تلتقط خطوات أعاده المسجلة](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="5cfd9-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="5cfd9-116">**ملاحظه**: تاكد من انك تلتقط عنوان تسجيل الدخول الخاص بالمستخدم المتاثر.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="5cfd9-117">جمع معلومات التفريغ الخاصة بالنسخة الاحتياطية و/أو الخطا (Windows).</span><span class="sxs-lookup"><span data-stu-id="5cfd9-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="5cfd9-118">شغل Windows Powershell علي الجهاز الذي تحدث فيه التعطل وشغل الأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="5cfd9-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="5cfd9-119">قم بإرفاق الملف بحاله الدعم.</span><span class="sxs-lookup"><span data-stu-id="5cfd9-119">Attach the file to your support case.</span></span>
