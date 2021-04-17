---
title: مشاكل في تسجيل الدخول إلى تطبيقات Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833011"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a><span data-ttu-id="9dcc1-102">شاشة تسجيل الدخول الفارغة في تطبيقات Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="9dcc1-102">Blank sign-in screen in Microsoft 365 apps</span></span>

<span data-ttu-id="9dcc1-103">لإصلاح هذه المشكلة، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="9dcc1-103">To fix this issue, try the following:</span></span>
- <span data-ttu-id="9dcc1-104">تثبيت التحديثات الأخيرة [لنظامي التشغيل Windows و](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="9dcc1-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="9dcc1-105">إعادة تعيين خيارات Internet Explorer: انتقل إلى أدوات خيارات الإنترنت المتقدمة إعادة تعيين إعدادات Internet Explorer (لاحظ أنك ستفقد الإعدادات المخصصة)، ثم حاول تسجيل الدخول  >    >    >   إلى Office مرة أخرى.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-105">Reset Internet Explorer options: Go to **Tools** > **Internet Options** > **Advanced** > **Reset Internet Explorer Settings** (note that you will lose custom settings), and then try signing in to Office again.</span></span>
- <span data-ttu-id="9dcc1-106">قم بتعطيل Windows Defender Application Guard (WDAG) أو أي برنامج مماثل لجدار الحماية أو برنامج مكافحة الفيروسات:</span><span class="sxs-lookup"><span data-stu-id="9dcc1-106">Disable the Windows Defender Application Guard (WDAG) or any similar firewall or anti-virus program:</span></span>
    1. <span data-ttu-id="9dcc1-107">في لوحة التحكم، انتقل إلى **البرامج**، ثم اختر **تشغيل ميزات Windows أو إيقاف تشغيلها**.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-107">In Control Panel, go to **Programs**, and then choose **Turn Windows features on or off**.</span></span>
    2. <span data-ttu-id="9dcc1-108">إذا تم تمكين Windows Defender Application Guard، فحاول تعطيله.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-108">If Windows Defender Application Guard is enabled, try disabling it.</span></span><br/>
    <span data-ttu-id="9dcc1-109">**ملاحظة:** قد تحتاج إلى إعادة تشغيل الكمبيوتر.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-109">**Note:** You may need to restart the computer.</span></span>
- <span data-ttu-id="9dcc1-110">تأكد من عدم حظر المكون الإضافية Microsoft.AAD.BrokerPlugin [AAD WAM](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) بواسطة أي تطبيق أو برنامج جدار حماية/مكافحة الفيروسات.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-110">Ensure that the Microsoft.AAD.BrokerPlugin [AAD WAM plug-in](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) is not being blocked by any application or firewall/anti-virus program.</span></span>
- <span data-ttu-id="9dcc1-111">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-111">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="9dcc1-112">**ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="9dcc1-112">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="9dcc1-113">(على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="9dcc1-113">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>

<span data-ttu-id="9dcc1-114">لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى [إصدار Office 2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="9dcc1-114">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>