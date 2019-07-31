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
- "2559"
ms.openlocfilehash: 5f500ecf1f779fb1be4d257fd050a3ad054087dc
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938120"
---
# <a name="fixing-the-office-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="76b23-102">تحديد الرسالة "الوحدة النمطية للنظام الأساسي الموثوق بها للكمبيوتر الخاص بك لا يعمل بشكل صحيح" تطبيقات Office</span><span class="sxs-lookup"><span data-stu-id="76b23-102">Fixing the Office apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="76b23-103">لإصلاح هذا الخطأ، جرب ما يلي:</span><span class="sxs-lookup"><span data-stu-id="76b23-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="76b23-104">تثبيت التحديثات ل [Windows](https://support.microsoft.com/help/4027667/windows-10-update) و [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span><span class="sxs-lookup"><span data-stu-id="76b23-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="76b23-105">["مكتب مسح" بيانات الاعتماد](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="76b23-105">[Clear Office credentials](https://docs.microsoft.com/eoffice/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="76b23-106">**ملاحظة:** لقد تغيرت المسارات لعام 2016 Office إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="76b23-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="76b23-107">(مثلاً: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="76b23-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="76b23-108">حاول [المستخدم عملية الاسترداد](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) لإصلاح فشل "الوحدة النمطية" النظام الأساسي الموثوق به (TPM).</span><span class="sxs-lookup"><span data-stu-id="76b23-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="76b23-109">تعيين انابليدال = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="76b23-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="76b23-110">زر الماوس الأيمن فوق الزر ابدأ في Windows، اختر **تشغيل**، اكتب **regedit**، وثم اختر **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="76b23-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="76b23-111">حدد **نعم** للسماح "محرر التسجيل" لإجراء تغييرات على الجهاز الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="76b23-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="76b23-112">في "محرر التسجيل"، إضافة قيمة DWORD **انابليدال** بإعداد **0** تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="76b23-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="76b23-113">لمزيد من المعلومات، راجع [اتصال مشكلات في تسجيل الدخول بعد التحديث إلى عام 2016 Office بناء 16.0.7967 على Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span><span class="sxs-lookup"><span data-stu-id="76b23-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>