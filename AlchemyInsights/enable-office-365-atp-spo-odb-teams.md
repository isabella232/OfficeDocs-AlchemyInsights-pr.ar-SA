---
title: تمكين Office 365 ATP SharePoint وأندريف وفرق Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32403020"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="c5264-102">تمكين الحماية من التهديدات المتقدمة 365 Office SharePoint على الإنترنت وأندريف وفرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="c5264-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="c5264-103">اذهب إلى https://protection.office.com وتسجيل الدخول.</span><span class="sxs-lookup"><span data-stu-id="c5264-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="c5264-104">اختر **إدارة التهديد** > **نهج** > **مرفقات آمنة**.</span><span class="sxs-lookup"><span data-stu-id="c5264-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="c5264-105">حدد **تشغيل ATP لفرق Microsoft SharePoint وأندريف،** ومن ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="c5264-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="c5264-106">(مستحسن) مسؤول عمومي أو كمسؤول SharePoint على الإنترنت، تشغيل cmdlet [سبوتينانت مجموعة](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) باستخدام المعلمة **ديسالووينفيكتيدفيليدوونلواد** تعيين إلى *true*.</span><span class="sxs-lookup"><span data-stu-id="c5264-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="c5264-107">(مستحسن) [إعداد تنبيهات](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.</span><span class="sxs-lookup"><span data-stu-id="c5264-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="c5264-108">سيتم ATP n ولفحص كل ملف واحد في SharePoint على الإنترنت أو أندريف أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="c5264-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="c5264-109">يتم تفحص الملفات بشكل غير متزامن، من خلال عملية تستخدم الأحداث نشاط المشاركة وضيوف، جنبا إلى جنب مع إشارات التهديد للتعرف على الملفات الضارة والأساليب البحثية الذكية.</span><span class="sxs-lookup"><span data-stu-id="c5264-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="c5264-110">راجع [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="c5264-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>