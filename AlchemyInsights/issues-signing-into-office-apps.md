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
- "2559"
ms.openlocfilehash: 4e7612562d036f1c717817d3c883d6df80f86e2f
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/05/2020
ms.locfileid: "44579852"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="1ede9-102">إصلاح تطبيقات Microsoft 365 "وحدة النظام الأساسي الموثوق بها للكمبيوتر لا تعمل بشكل صحيح" الرسالة</span><span class="sxs-lookup"><span data-stu-id="1ede9-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="1ede9-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1ede9-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="1ede9-104">تثبيت آخر التحديثات [لـ Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="1ede9-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="1ede9-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="1ede9-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="1ede9-106">**ملاحظة:** تم تغيير مسارات التسجيل لـ Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="1ede9-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="1ede9-107">(على سبيل: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="1ede9-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="1ede9-108">جرّب [عملية استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح فشل وحدة النظام الأساسي الموثوق بها (TPM).</span><span class="sxs-lookup"><span data-stu-id="1ede9-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="1ede9-109">تعيين EnableADAL = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1ede9-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="1ede9-110">انقر بزر بدء تشغيل Windows، واختر **تشغيل،** واكتب **regedit،** ثم اختر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1ede9-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="1ede9-111">حدد **نعم** للسماح لمحرر التسجيل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="1ede9-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="1ede9-112">في محرر التسجيل، قم بإضافة قيمة DWORD من **EnableADAL** مع إعداد **0** تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="1ede9-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="1ede9-113">لمزيد من المعلومات، راجع [مشكلات "تسجيل الدخول" في "الاتصال" بعد التحديث إلى Office 2016 بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="1ede9-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>