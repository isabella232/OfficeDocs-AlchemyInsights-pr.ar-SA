---
title: مشاكل تسجيل الدخول إلى تطبيقات Microsoft 365
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
- "2559"
ms.openlocfilehash: d736c6c687695824f0ab37b8ffdc8456065353b0
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709093"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="926b8-102">إصلاح رسالة تطبيقات Microsoft 365 "الوحدة النمطية ل "النظام الأساسي الموثوق به" على الكمبيوتر لا تعمل بشكل صحيح</span><span class="sxs-lookup"><span data-stu-id="926b8-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="926b8-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="926b8-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="926b8-104">تثبيت آخر التحديثات [لنظامي التشغيل Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="926b8-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="926b8-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="926b8-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="926b8-106">**ملاحظة:** تم تغيير مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="926b8-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="926b8-107">(على Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="926b8-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="926b8-108">جرب عملية [استرداد المستخدم لإصلاح](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) حالات فشل الوحدة النمطية (TPM) الموثوق بها في النظام الأساسي.</span><span class="sxs-lookup"><span data-stu-id="926b8-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="926b8-109">قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="926b8-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="926b8-110">انقر بزر الماوس الأيمن فوق الزر "ابدأ" في Windows، واختر **"تشغيل"،** ثم اكتب **regedit،** ثم اختر **"موافق".**</span><span class="sxs-lookup"><span data-stu-id="926b8-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="926b8-111">حدد **"نعم"** للسماح ل "محرر السجل" بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="926b8-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="926b8-112">في "محرر السجل"، أضف قيمة DWORD ل **EnableADAL** بإعداد **0** ضمن HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="926b8-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="926b8-113">لمزيد من المعلومات، راجع مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى [Office 2016 إصدار 16.0.7967 على Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="926b8-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>