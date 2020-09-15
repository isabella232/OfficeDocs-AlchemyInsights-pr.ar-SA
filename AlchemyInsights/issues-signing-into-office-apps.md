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
- "2559"
ms.openlocfilehash: 57a4df23dc66eaf4c283dde741be6f415939633d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695166"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="1df32-102">إصلاح تطبيقات Microsoft 365 "الوحدة النمطية للنظام الأساسي الموثوق به للكمبيوتر لا تعمل بشكل صحيح"</span><span class="sxs-lookup"><span data-stu-id="1df32-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="1df32-103">لإصلاح هذا الخطأ، حاول القيام بالخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1df32-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="1df32-104">تثبيت آخر التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="1df32-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="1df32-105">[مسح بيانات اعتماد Office](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام "أداره بيانات اعتماد Windows".</span><span class="sxs-lookup"><span data-stu-id="1df32-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="1df32-106">**ملاحظه:** لقد تغيرت مسارات التسجيل ل Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="1df32-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="1df32-107">(علي سبيل المثال: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="1df32-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="1df32-108">جرب [عمليه استرداد المستخدم](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح حالات فشل الوحدة النمطية للنظام الأساسي الموثوق به (TPM).</span><span class="sxs-lookup"><span data-stu-id="1df32-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="1df32-109">عين EnableADAL = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="1df32-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="1df32-110">انقر بزر الماوس الأيمن فوق "بدء" في Windows ، واختر **تشغيل**، واكتب **regedit**، ثم اختر **موافق**.</span><span class="sxs-lookup"><span data-stu-id="1df32-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="1df32-111">حدد **نعم** للسماح لمحرر التسجيل باجراء تغييرات علي جهازك.</span><span class="sxs-lookup"><span data-stu-id="1df32-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="1df32-112">في "محرر السجل" ، أضف قيمه DWORD ل **EnableADAL** باستخدام اعداد **0** ضمن HKEY_CURRENT_USER \software\microsoft\office\16.0\common\identity.</span><span class="sxs-lookup"><span data-stu-id="1df32-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="1df32-113">لمزيد من المعلومات ، راجع [مشاكل الاتصال في تسجيل الدخول بعد التحديث إلى Office 2016 16.0.7967 علي Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="1df32-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>