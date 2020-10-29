---
title: تمكين Office 365 ATP لفرق SharePoint و OneDrive و Microsoft
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
ms.openlocfilehash: bef43656097c6f27677172899df1ada7900a9b64
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801034"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="72fde-102">تمكين Microsoft Defender ل Office 365 for SharePoint Online و OneDrive و Microsoft</span><span class="sxs-lookup"><span data-stu-id="72fde-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="72fde-103">انتقل إلى https://protection.office.com وسجل الدخول.</span><span class="sxs-lookup"><span data-stu-id="72fde-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="72fde-104">اختر **Threat management**  >  **Policy**  >  **المرفقات الامنه** لنهج أداره المخاطر.</span><span class="sxs-lookup"><span data-stu-id="72fde-104">Choose **Threat management** > **Policy** > **Safe Attachments** .</span></span>
3. <span data-ttu-id="72fde-105">حدد **تشغيل ATP لفرق SharePoint و OneDrive و Microsoft** ، ثم انقر فوق **حفظ** .</span><span class="sxs-lookup"><span data-stu-id="72fde-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams** , and then click **Save** .</span></span>
4. <span data-ttu-id="72fde-106">مطلوب بصفتك مسؤولا عاما أو مسؤول SharePoint Online ، قم بتشغيل الأمر cmdlet [سبوتينانت](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **ديسالووينفيكتيدفيليدوونلواد** إلى *true* .</span><span class="sxs-lookup"><span data-stu-id="72fde-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true* .</span></span>
5. <span data-ttu-id="72fde-107">مطلوب [اعداد التنبيات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.</span><span class="sxs-lookup"><span data-stu-id="72fde-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="72fde-108">سيقوم ATP بفحص كل ملف واحد في SharePoint Online أو OneDrive أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="72fde-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="72fde-109">يتم مسح الملفات بشكل غير متزامن ، من خلال عمليه تستخدم احداث نشاط المشاركة والضيف ، إلى جانب المعرفات الذكية وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="72fde-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="72fde-110">راجع [ATP لفرق SharePoint و OneDrive و Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="72fde-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>