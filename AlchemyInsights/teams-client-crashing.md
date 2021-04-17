---
title: هل يتوقف عميل Teams عن العمل؟
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
- "9002323"
- "4512"
ms.openlocfilehash: 20f03b075787cab85ab15d5272c0416b88ebbaee
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826258"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="42b97-102">هل يتوقف عميل Teams عن العمل؟</span><span class="sxs-lookup"><span data-stu-id="42b97-102">Teams client crashing?</span></span>

<span data-ttu-id="42b97-103">إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="42b97-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="42b97-104">إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="42b97-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="42b97-105">تأكد من إمكانية الوصول إلى كل عناوين URL في [Microsoft 365](https://docs.microsoft.com/microsoftteams/connectivity-issues) ونطاقات عناوينه.</span><span class="sxs-lookup"><span data-stu-id="42b97-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="42b97-106">سجل الدخول باستخدام حساب مسؤول [](https://docs.microsoft.com/office365/enterprise/view-service-health) المستأجر وتحقق من لوحة معلومات حالة الخدمة للتحقق من عدم وجود انقطاع أو انخفاض في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="42b97-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="42b97-107">إلغاء تثبيت تطبيق Teams (ارتباط) وإعادة تثبيته</span><span class="sxs-lookup"><span data-stu-id="42b97-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="42b97-108">استعرض بحثا عن المجلد ٪appdata٪\Microsoft\teams\ على الكمبيوتر واحذف كل الملفات الموجودة في ذلك الدليل.</span><span class="sxs-lookup"><span data-stu-id="42b97-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="42b97-109">[قم بتنزيل تطبيق Teams وتثبيته،](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)وإذا أمكن، قم بتثبيت Teams كمسؤول (انقر بزر الماوس الأيمن فوق مثبت Teams وحدد "تشغيل كمسؤول" إذا كان متوفرا).</span><span class="sxs-lookup"><span data-stu-id="42b97-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="42b97-110">إذا كان عميل Teams لا يزال يعطل، هل يمكنك إعادة إنتاج المشكلة؟</span><span class="sxs-lookup"><span data-stu-id="42b97-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="42b97-111">إذا كان الأمر كذلك:</span><span class="sxs-lookup"><span data-stu-id="42b97-111">If so:</span></span>

1. <span data-ttu-id="42b97-112">استخدم "مسجل الخطوات" لتسجيل الخطوات.</span><span class="sxs-lookup"><span data-stu-id="42b97-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="42b97-113">أغلق جميع التطبيقات السرية أو غير الضرورية.</span><span class="sxs-lookup"><span data-stu-id="42b97-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="42b97-114">تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="42b97-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="42b97-115">[قم بجمع سجلات الفرق التي تسجل خطوات إعادة الحماية المسجلة](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="42b97-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="42b97-116">**ملاحظة:** تأكد من تسجيل عنوان تسجيل الدخول للمستخدم الذي تم التأثير عليه.</span><span class="sxs-lookup"><span data-stu-id="42b97-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="42b97-117">جمع معلومات مستودع تفريغ و/أو خطأ (Windows).</span><span class="sxs-lookup"><span data-stu-id="42b97-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="42b97-118">تشغيل Windows Powershell على الجهاز الذي يحدث فيه العطل وتشغيل الأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="42b97-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="42b97-119">أرفق الملف بقضيه الدعم.</span><span class="sxs-lookup"><span data-stu-id="42b97-119">Attach the file to your support case.</span></span>
