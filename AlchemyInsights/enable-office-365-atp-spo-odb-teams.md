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
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703413"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="ef435-102">تمكين Office 365 حماية متقدمة من التهديدات لفرق SharePoint Online وOneDrive وMicrosoft</span><span class="sxs-lookup"><span data-stu-id="ef435-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="ef435-103">اذهب https://protection.office.com إلى وتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="ef435-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="ef435-104">اختر**مرفقات\*\*\*\*آمنة لسياسة** >  **إدارة** > التهديدات.</span><span class="sxs-lookup"><span data-stu-id="ef435-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="ef435-105">حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="ef435-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="ef435-106">(موصى به) كمسؤول عمومي أو مسؤول SharePoint عبر الإنترنت، قم بتشغيل [cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين معلمة **FileFileDownload غير مسموح** بها إلى *صواب*.</span><span class="sxs-lookup"><span data-stu-id="ef435-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="ef435-107">(موصى به) [إعداد تنبيهات](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم اكتشافها.</span><span class="sxs-lookup"><span data-stu-id="ef435-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="ef435-108">سوف ATP nto مسح كل ملف واحد في SharePoint عبر الإنترنت أو OneDrive أو Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="ef435-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="ef435-109">يتم مسح الملفات ضوئيًا بشكل غير متزامن، من خلال عملية تستخدم أحداث المشاركة وأحداث نشاط الضيف، بالإضافة إلى الاستدلالات الذكية وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="ef435-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="ef435-110">راجع [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="ef435-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>