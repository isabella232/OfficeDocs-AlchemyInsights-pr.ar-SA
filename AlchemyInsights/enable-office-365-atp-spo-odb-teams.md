---
title: تمكين Office 365 ATP لفرق SharePoint وOneDrive وMicrosoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506905"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="096fe-102">تمكين Office 365 حماية متقدمة من التهديدات لفرق SharePoint Online وOneDrive وMicrosoft</span><span class="sxs-lookup"><span data-stu-id="096fe-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="096fe-103">اذهب إلى https://protection.office.com وتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="096fe-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="096fe-104">اختر **Threat management**  >  مرفقات آمنة لسياسة**إدارة**  >  **Safe Attachments**التهديدات.</span><span class="sxs-lookup"><span data-stu-id="096fe-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="096fe-105">حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="096fe-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="096fe-106">(موصى به) كمسؤول عمومي أو مسؤول SharePoint عبر الإنترنت، قم بتشغيل [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين معلمة **FileFileDownload غير مسموح** بها إلى *صواب*.</span><span class="sxs-lookup"><span data-stu-id="096fe-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="096fe-107">(موصى به) [إعداد تنبيهات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم اكتشافها.</span><span class="sxs-lookup"><span data-stu-id="096fe-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="096fe-108">سوف ATP nto مسح كل ملف واحد في SharePoint عبر الإنترنت أو OneDrive أو Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="096fe-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="096fe-109">يتم مسح الملفات ضوئيًا بشكل غير متزامن، من خلال عملية تستخدم أحداث المشاركة وأحداث نشاط الضيف، بالإضافة إلى الاستدلالات الذكية وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="096fe-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="096fe-110">راجع [ATP لـ SharePoint و OneDrive وفرق Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="096fe-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>