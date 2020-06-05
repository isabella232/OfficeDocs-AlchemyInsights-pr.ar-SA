---
title: مشكلات تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 4658b4df8a48072b4cc9d72bf503d7911bb5126b
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579888"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="ab190-102">شاشة تسجيل الدخول الفارغة في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="ab190-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="ab190-103">لإصلاح هذه المشكلة، حاول ما يلي:</span><span class="sxs-lookup"><span data-stu-id="ab190-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="ab190-104">تثبيت آخر التحديثات [لـ Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="ab190-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="ab190-105">إعادة تعيين خيارات Internet **Tools**Explorer: انتقل إلى  >  **أدوات خيارات إنترنت**  >  **Advanced**  >  **المتقدمة إعادة تعيين إعدادات إنترنت إكسبلورر** (لاحظ أنك سوف تفقد الإعدادات المخصصة)، ومن ثم حاول تسجيل الدخول إلى Office مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="ab190-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="ab190-106">تعطيل حارس تطبيق Windows Defender (WDAG) أو أي جدار حماية مماثل أو برنامج مضاد للفيروسات:</span><span class="sxs-lookup"><span data-stu-id="ab190-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="ab190-107">في لوحة التحكم، انتقل إلى **البرامج،** ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.</span><span class="sxs-lookup"><span data-stu-id="ab190-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="ab190-108">إذا تم تمكين Windows Defender Application Guard، فحاول تعطيله.</span><span class="sxs-lookup"><span data-stu-id="ab190-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="ab190-109">**ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="ab190-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="ab190-110">تأكد من أن Microsoft.AAD.BrokerPlugin [AAD WAM المكونات في](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) لا يتم حظرها من قبل أي تطبيق أو جدار الحماية / برنامج مكافحة الفيروسات.</span><span class="sxs-lookup"><span data-stu-id="ab190-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="ab190-111">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="ab190-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="ab190-112">**ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="ab190-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="ab190-113">(على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="ab190-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="ab190-114">لمزيد من المعلومات، راجع [مشكلات "تسجيل الدخول" في "الاتصال" بعد التحديث إلى Office 2016 بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="ab190-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>