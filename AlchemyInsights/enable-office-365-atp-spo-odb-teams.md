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
ms.openlocfilehash: c84458622ae86bcf0f9f541a3a209b4f0ff2fc3f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709894"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="82fd4-102">تمكين الحماية المتقدمة من المخاطر ل Office 365 لفرق SharePoint Online و OneDrive و Microsoft</span><span class="sxs-lookup"><span data-stu-id="82fd4-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="82fd4-103">انتقل إلى https://protection.office.com وسجل الدخول.</span><span class="sxs-lookup"><span data-stu-id="82fd4-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="82fd4-104">اختر **Threat management**  >  **Policy**  >  **المرفقات الامنه**لنهج أداره المخاطر.</span><span class="sxs-lookup"><span data-stu-id="82fd4-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="82fd4-105">حدد **تشغيل ATP لفرق SharePoint و OneDrive و Microsoft**، ثم انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="82fd4-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="82fd4-106">مطلوب بصفتك مسؤولا عاما أو مسؤول SharePoint Online ، قم بتشغيل الأمر cmdlet [سبوتينانت](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) مع تعيين المعلمة **ديسالووينفيكتيدفيليدوونلواد** إلى *true*.</span><span class="sxs-lookup"><span data-stu-id="82fd4-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="82fd4-107">مطلوب [اعداد التنبيات](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.</span><span class="sxs-lookup"><span data-stu-id="82fd4-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="82fd4-108">سيقوم ATP بفحص كل ملف واحد في SharePoint Online أو OneDrive أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="82fd4-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="82fd4-109">يتم مسح الملفات بشكل غير متزامن ، من خلال عمليه تستخدم احداث نشاط المشاركة والضيف ، إلى جانب المعرفات الذكية وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="82fd4-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="82fd4-110">راجع [ATP لفرق SharePoint و OneDrive و Microsoft](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="82fd4-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>