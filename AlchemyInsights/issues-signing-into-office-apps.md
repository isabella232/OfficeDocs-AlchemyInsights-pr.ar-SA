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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51832990"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="068da-102">إصلاح رسالة تطبيقات Microsoft 365 "وحدة النظام الأساسي الموثوق بها في الكمبيوتر لا تعمل بشكل صحيح"</span><span class="sxs-lookup"><span data-stu-id="068da-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="068da-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="068da-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="068da-104">تثبيت التحديثات الأخيرة [لنظامي التشغيل Windows و](https://support.microsoft.com/help/4027667/windows-10-update) [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="068da-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="068da-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="068da-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="068da-106">**ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="068da-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="068da-107">(على ما يلي: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="068da-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="068da-108">جرب عملية [استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح حالات فشل وحدة النظام الأساسي الموثوق بها (TPM).</span><span class="sxs-lookup"><span data-stu-id="068da-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="068da-109">قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="068da-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="068da-110">انقر بزر الماوس الأيمن فوق زر البدء في Windows، واختر **تشغيل**، وا اكتب **regedit**، ثم اختر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="068da-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="068da-111">حدد **نعم** للسماح لمحرر السجل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="068da-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="068da-112">في محرر السجل، أضف قيمة DWORD **من EnableADAL** بإعداد **0** ضمن HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="068da-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="068da-113">لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى [إصدار Office 2016 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="068da-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>