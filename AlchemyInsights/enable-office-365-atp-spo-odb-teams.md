---
title: تمكين Office 365 ATP SharePoint OneDrive و Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: dd367176f8d6f38f1f94ae6627229234f15c81ff
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543915"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="adc10-102">تمكين Microsoft Defender Office 365 SharePoint عبر الإنترنت OneDrive و Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="adc10-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="adc10-103">انتقل إلى https://protection.office.com ثم سجل الدخول.</span><span class="sxs-lookup"><span data-stu-id="adc10-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="adc10-104">اختر **المرفقات الآمنة**  >  **لن نهج** إدارة  >  **المخاطر.**</span><span class="sxs-lookup"><span data-stu-id="adc10-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="adc10-105">حدد **تشغيل Defender Office 365 SharePoint** OneDrive و Microsoft Teams ، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="adc10-105">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="adc10-106">(مستحسن) كمسؤول عام أو مسؤول SharePoint Online، قم بتشغيل الأمر [Cmdlet Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **DisallowInfectedFileDownload** إلى *true*.</span><span class="sxs-lookup"><span data-stu-id="adc10-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="adc10-107">(مستحسن) [إعداد التنبيهات](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.</span><span class="sxs-lookup"><span data-stu-id="adc10-107">(Recommended) [Set up alerts](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="adc10-108">لن يقوم Microsoft Defender Office 365 بفحص كل ملف في SharePoint أو OneDrive أو Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="adc10-108">Microsoft Defender for Office 365 will not scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="adc10-109">يتم فحص الملفات بشكل غير متزامن، من خلال عملية تستخدم أحداث نشاط الضيف والمشاركة، إلى جانب مؤشرات بحث ذكية وإشارات تهديدات لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="adc10-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="adc10-110">راجع [Microsoft Defender Office 365 SharePoint OneDrive و Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="adc10-110">See [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>