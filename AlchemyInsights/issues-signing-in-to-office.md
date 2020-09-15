---
title: المشاكل المتعلقة بتسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 3c016b198ad43f35c8149dde71c28a2f7fc3bd38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695274"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="7ae45-102">شاشه تسجيل الدخول الفارغة في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="7ae45-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="7ae45-103">لإصلاح هذه المشكلة ، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="7ae45-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="7ae45-104">تثبيت آخر التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="7ae45-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="7ae45-105">أعاده تعيين خيارات internet explorer: **Tools**انتقل إلى  >  **أدوات الإنترنت خيارات**  >  أعاده تعيين**متقدمة**  >  **لإعدادات internet Explorer** (لاحظ انك ستفقد الإعدادات المخصصة) ، ثم حاول تسجيل الدخول إلى Office مره أخرى.</span><span class="sxs-lookup"><span data-stu-id="7ae45-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="7ae45-106">تعطيل ' حماية التطبيقات ل Windows Defender ' (فداج) أو اي برنامج جدار حماية مشابه أو برامج مكافحه الفيروسات:</span><span class="sxs-lookup"><span data-stu-id="7ae45-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="7ae45-107">في لوحه التحكم ، انتقل إلى **البرامج**، ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.</span><span class="sxs-lookup"><span data-stu-id="7ae45-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="7ae45-108">إذا تم تمكين حماية التطبيقات ل Windows Defender ، فجرب تعطيلها.</span><span class="sxs-lookup"><span data-stu-id="7ae45-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="7ae45-109">**ملاحظه:** قد تحتاج إلى أعاده تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="7ae45-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="7ae45-110">تاكد من انه لم يتم حظر [المكون الإضافي بروكيربلوجين aad](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) الخاص ب aad ، بواسطة اي تطبيق أو جدار حماية/برنامج مكافحه الفيروسات.</span><span class="sxs-lookup"><span data-stu-id="7ae45-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="7ae45-111">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".</span><span class="sxs-lookup"><span data-stu-id="7ae45-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="7ae45-112">**ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="7ae45-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="7ae45-113">(علي سبيل المثال: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="7ae45-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="7ae45-114">لمزيد من المعلومات ، راجع [مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 16.0.7967 علي Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="7ae45-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>