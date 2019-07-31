---
title: مشكلات تسجيل الدخول إلى تطبيقات Office
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
ms.openlocfilehash: 08bb0a94066f071f2ba0e9c54378f0d479191496
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938119"
---
# <a name="blank-sign-in-screen-in-office-apps"></a><span data-ttu-id="a076b-102">شاشة تسجيل الدخول فارغة في تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="a076b-102">Blank sign-in screen in Office apps</span></span>

<span data-ttu-id="a076b-103">لحل هذه المشكلة، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="a076b-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="a076b-104">تثبيت التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="a076b-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="a076b-105">إعادة تعيين خيارات Internet Explorer: انتقل إلى **أدوات** > **خيارات إنترنت** > **خيارات متقدمة** > **إعادة تعيين إعدادات Internet Explorer** (لاحظ أنك ستفقد إعدادات مخصصة)، وثم حاول تسجيل الدخول إلى Office مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="a076b-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="a076b-106">تعطيل حماية التطبيق Windows Defender (وداج) أو أي برنامج جدار حماية أو برنامج مكافحة الفيروسات مشابهة:</span><span class="sxs-lookup"><span data-stu-id="a076b-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="a076b-107">في "لوحة التحكم"، انتقل إلى **البرامج**، وثم اختر **تشغيل ميزات Windows أو إيقاف تشغيله**.</span><span class="sxs-lookup"><span data-stu-id="a076b-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="a076b-108">إذا تم تمكين حماية التطبيق Windows Defender، حاول تعطيله.</span><span class="sxs-lookup"><span data-stu-id="a076b-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="a076b-109">**ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="a076b-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="a076b-110">تأكد من أن Microsoft.AAD.BrokerPlugin [أم عاد المكون الإضافي](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) لا يتم حظر من قبل أي تطبيق أو برنامج جدار حماية/المضادة للفيروسات.</span><span class="sxs-lookup"><span data-stu-id="a076b-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="a076b-111">["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="a076b-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="a076b-112">**ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="a076b-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="a076b-113">(مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="a076b-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="a076b-114">لمزيد من المعلومات، راجع [اتصال مشكلات في تسجيل الدخول بعد التحديث إلى عام 2016 Office بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="a076b-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>