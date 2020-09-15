---
title: ATP لفرق SharePoint و OneDrive و Microsoft
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 3d02ded959114675847831690b4d4a3ebcf0e137
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715548"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="2afd4-102">ATP لفرق SharePoint و OneDrive و Microsoft</span><span class="sxs-lookup"><span data-stu-id="2afd4-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="2afd4-103">اتبع هذه الخطوات لتمكين الحماية المتقدمة من المخاطر:</span><span class="sxs-lookup"><span data-stu-id="2afd4-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="2afd4-104">انتقل إلى [https://protection.office.com](https://protection.office.com) وقم بتسجيل الدخول باستخدام حساب مسؤول الأمان أو المسؤول العام.</span><span class="sxs-lookup"><span data-stu-id="2afd4-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="2afd4-105">في جزء التنقل الأيمن ضمن **أداره التهديدات**، اختر **Policy** \> **المرفقات الامنه**للنهج.</span><span class="sxs-lookup"><span data-stu-id="2afd4-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="2afd4-106">حدد **تشغيل ATP لفرق SharePoint و OneDrive و Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="2afd4-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="2afd4-107">[يمكنك إنشاء نهج تنبيه](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) لتلقي اعلامات عند اكتشاف الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="2afd4-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="2afd4-108">للحصول علي الإرشادات الكاملة ، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2afd4-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="2afd4-109">**ملاحظه**: لا يقوم ATP بفحص كل ملف فردي في SharePoint Online أو OneDrive for Business أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="2afd4-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="2afd4-110">يتم مسح الملفات بشكل غير متزامن بواسطة عمليه تستخدم الإشارات نشاط المشاركة ونشاط الضيوف والمخاطر لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="2afd4-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="2afd4-111">لمزيد من المعلومات ، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2afd4-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
