---
title: Teams تعطل العميل
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
ms.openlocfilehash: 7acb2f5f87a9cfbd67cd94efca696665fd80fc4a
ms.sourcegitcommit: 3cdfde87b7311c200431196031af92c640fd0d8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/29/2021
ms.locfileid: "53187708"
---
# <a name="teams-client-crashing"></a><span data-ttu-id="1d5a5-102">Teams تعطل العميل</span><span class="sxs-lookup"><span data-stu-id="1d5a5-102">Teams client crashing</span></span>

<span data-ttu-id="1d5a5-103">إذا كان عميل Teams يتوقف عن العمل، فحاول القيام بما يلي:</span><span class="sxs-lookup"><span data-stu-id="1d5a5-103">If your Teams client is crashing, try the following:</span></span>

- <span data-ttu-id="1d5a5-104">إذا كنت تستخدم تطبيق سطح المكتب من Teams، [فتأكد من تحديث البرنامج بشكل كامل](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span><span class="sxs-lookup"><span data-stu-id="1d5a5-104">If you are using the Teams desktop app, [make sure the app is fully updated](https://support.office.com/article/Update-Microsoft-Teams-535a8e4b-45f0-4f6c-8b3d-91bca7a51db1).</span></span>

- <span data-ttu-id="1d5a5-105">تأكد من إمكانية Microsoft 365 [عناوين URL ونطاقات](/microsoftteams/connectivity-issues) العنوان.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-105">Make sure all the [Microsoft 365 URLs and address ranges](/microsoftteams/connectivity-issues) are accessible.</span></span>

- <span data-ttu-id="1d5a5-106">سجل الدخول باستخدام حساب مسؤول [](/office365/enterprise/view-service-health) المستأجر وتحقق من لوحة معلومات حالة الخدمة للتحقق من عدم وجود انقطاع أو انخفاض في الخدمة.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-106">Log in with your tenant admin account and check your [Service Health Dashboard](/office365/enterprise/view-service-health) to verify that no outage or service degradation exists.</span></span>

- <span data-ttu-id="1d5a5-107">إلغاء تثبيت التطبيق Teams تثبيته</span><span class="sxs-lookup"><span data-stu-id="1d5a5-107">Uninstall and reinstall the Teams Application</span></span>
    - <span data-ttu-id="1d5a5-108">استعرض إلى المجلد ٪appdata٪\Microsoft\Teams\ على الكمبيوتر واحذف كل الملفات الموجودة في ذلك الدليل.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-108">Browse to the %appdata%\Microsoft\Teams\ folder on your computer and delete all files in that directory.</span></span>
    - <span data-ttu-id="1d5a5-109">[قم بتنزيل Teams التطبيق](https://www.microsoft.com/microsoft-teams/download-app)، وإذا أمكن، Teams كمسؤول (انقر بزر الماوس الأيمن فوق مثبت Teams، وحدد تشغيل كمسؤول إذا كان متوفرا). </span><span class="sxs-lookup"><span data-stu-id="1d5a5-109">[Download and install the Teams App](https://www.microsoft.com/microsoft-teams/download-app), and if possible, install Teams as an administrator (right-click the Teams installer, and select **Run as administrator** if available).</span></span>

<span data-ttu-id="1d5a5-110">إذا كان Teams العميل لا يزال يعطل، فحاول إعادة إنتاج المشكلة.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-110">If your Teams client is still crashing, try to reproduce the issue.</span></span> <span data-ttu-id="1d5a5-111">إذا كان ممكنا:</span><span class="sxs-lookup"><span data-stu-id="1d5a5-111">If you can:</span></span>

1. <span data-ttu-id="1d5a5-112">استخدم "مسجل الخطوات" لتسجيل الخطوات.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-112">Use the Steps Recorder to capture your steps.</span></span>
    - <span data-ttu-id="1d5a5-113">أغلق جميع التطبيقات السرية أو غير الضرورية.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-113">Close ALL unnecessary or confidential applications.</span></span>
    - <span data-ttu-id="1d5a5-114">تشغيل مسجل الخطوات وإعادة إنتاج المشكلة أثناء تسجيل الدخول باستخدام حساب المستخدم المتأثر.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-114">Launch the Steps Recorder and reproduce the issue while logged in with the affected user account.</span></span>
    - <span data-ttu-id="1d5a5-115">[قم بجمع سجلات الفرق التي تسجل خطوات إعادة الحماية المسجلة](/microsoftteams/log-files).</span><span class="sxs-lookup"><span data-stu-id="1d5a5-115">[Collect the teams logs that capture the recorded repro steps](/microsoftteams/log-files).</span></span> <span data-ttu-id="1d5a5-116">**ملاحظة:** تأكد من تسجيل عنوان تسجيل الدخول للمستخدم الذي تم التأثير عليه.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-116">**Note**: Make sure you capture the sign-in address of the impacted user.</span></span>
    - <span data-ttu-id="1d5a5-117">تجميع معلومات مستودع تفريغ و/أو خطأ (Windows).</span><span class="sxs-lookup"><span data-stu-id="1d5a5-117">Collect the dump and/or Fault bucket info (Windows).</span></span> <span data-ttu-id="1d5a5-118">تشغيل Windows Powershell على الجهاز الذي يحدث فيه العطل وتشغيل الأوامر التالية (بعد كل أمر، اضغط على Enter):</span><span class="sxs-lookup"><span data-stu-id="1d5a5-118">Launch Windows Powershell on the machine where the crash is occurring and run the following commands (after each command, press Enter):</span></span>

    <span data-ttu-id="1d5a5-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span><span class="sxs-lookup"><span data-stu-id="1d5a5-119">`cd $env:temp` `Get-EventLog -LogName Application -Message "*Teams.exe*" -InstanceId 1001 | Select-Object -First 10 | Format-List > FaultBuckets.txt`</span></span>
    `notepad .\FaultBuckets.txt`
    
2. <span data-ttu-id="1d5a5-120">بعد إنشاء الملف النصي ويظهر على الشاشة، احفظ الملف وأرفقه بطلب الخدمة.</span><span class="sxs-lookup"><span data-stu-id="1d5a5-120">After the text file is generated and appears on your screen, save the file and attach it to the service request.</span></span> 
