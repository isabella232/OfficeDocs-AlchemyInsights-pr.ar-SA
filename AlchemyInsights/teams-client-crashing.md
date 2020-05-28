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
ms.openlocfilehash: ac1cc05adfa33626ff34d30dca6c77f1bb96477a
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/23/2020
ms.locfileid: "44354039"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="2a2fd-102">هل يتوقف عميل Teams عن العمل؟</span><span class="sxs-lookup"><span data-stu-id="2a2fd-102">Teams client crashing?</span></span>

<span data-ttu-id="2a2fd-103">إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="2a2fd-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="2a2fd-104">إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="2a2fd-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="2a2fd-105">تأكد من إمكانية الوصول إلى كافة [عناوين URL ونطاقات العناوين من Microsoft 365.](https://docs.microsoft.com/microsoftteams/connectivity-issues)</span><span class="sxs-lookup"><span data-stu-id="2a2fd-105">Make sure all the [Microsoft 365 URLs and address ranges](https://docs.microsoft.com/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="2a2fd-106">سجّل الدخول باستخدام حساب مسؤول المستأجر وتحقق من [لوحة معلومات صحة الخدمة](https://docs.microsoft.com/office365/enterprise/view-service-health) للتحقق من عدم وجود انقطاع أو تدهور في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-106">Log in with your tenant admin account and check your [Service Health Dashboard](https://docs.microsoft.com/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="2a2fd-107">إلغاء تثبيت تطبيق الفرق وإعادة تثبيته (رابط)</span><span class="sxs-lookup"><span data-stu-id="2a2fd-107">Uninstall and reinstall the Teams Application (link)</span></span>
    - <span data-ttu-id="2a2fd-108">استعراض إلى %appdata%\Microsoft\teams\المجلد على جهاز الكمبيوتر الخاص بك وحذف كافة الملفات في هذا الدليل.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-108">Browse to the %appdata%\Microsoft\teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="2a2fd-109">[قم بتنزيل تطبيق Teams وتثبيته](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy)، وإذا كان ذلك ممكنًا ، قم بتثبيت Teams كمسؤول (انقر على مثبت الفرق وحدد "تشغيل كمسؤول" إذا كان متاحًا).</span><span class="sxs-lookup"><span data-stu-id="2a2fd-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-365/microsoft-teams/group-chat-software#office-DesktopAppDownload-ofoushy), and if possible, install Teams as an administrator (right click the Teams installer and select "Run as administrator" if available).</span></span>

<span data-ttu-id="2a2fd-110">إذا كان عميل Teams لا يزال يتعطل، هل يمكنك إعادة إنشاء المشكلة؟</span><span class="sxs-lookup"><span data-stu-id="2a2fd-110">If your Teams client is still crashing, can you reproduce the issue?</span></span> <span data-ttu-id="2a2fd-111">إذا كان الأمر كذلك:</span><span class="sxs-lookup"><span data-stu-id="2a2fd-111">If so:</span></span>

1. <span data-ttu-id="2a2fd-112">استخدم مسجل الخطوات لالتقاط خطواتك.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="2a2fd-113">إغلاق كافة التطبيقات غير الضرورية أو السرية.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="2a2fd-114">تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="2a2fd-115">[جمع سجلات الفرق التي تلتقط الخطوات repro المسجلة](https://docs.microsoft.com/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="2a2fd-115">[Collect the teams logs that capture the recorded repro steps](https://docs.microsoft.com/microsoftteams/log-files).</span></span> <span data-ttu-id="2a2fd-116">**ملاحظة:** تأكد من التقاط عنوان تسجيل الدخول للمستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="2a2fd-117">جمع تفريغ و / أو خطأ دلو معلومات (ويندوز).</span><span class="sxs-lookup"><span data-stu-id="2a2fd-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="2a2fd-118">تشغيل Windows Powershell على الجهاز حيث يحدث التعطل وتشغيل الأوامر التالية:</span><span class="sxs-lookup"><span data-stu-id="2a2fd-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands:</span></span>

        `
        PS C:\Users\user01> cd $env:temp
        PS C:\Users\user01\AppData\Local\Temp> Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt
        PS C:\Users\user01\AppData\Local\Temp> notepad .\FaultBuckets.txt
        `
    
2. <span data-ttu-id="2a2fd-119">إرفاق الملف بحالة الدعم الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="2a2fd-119">Attach the file to your support case.</span></span>
