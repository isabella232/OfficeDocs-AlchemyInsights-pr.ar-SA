---
title: ATP SharePoint وأندريف وفرق Microsoft
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764794"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="5e6e4-102">ATP SharePoint وأندريف وفرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="5e6e4-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="5e6e4-103">اتبع هذه الخطوات لتمكين "المتقدمة الحماية من التهديدات":</span><span class="sxs-lookup"><span data-stu-id="5e6e4-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="5e6e4-104">اذهب إلى [https://protection.office.com](https://protection.office.com) وتسجيل الدخول باستخدام المسؤول العمومي أو حساب مسؤول الأمن.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="5e6e4-105">في جزء التنقل الأيمن ضمن **إدارة التهديد**، اختيار **نهج** \> **مرفقات آمنة**.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="5e6e4-106">حدد **تشغيل ATP SharePoint وأندريف، وفرق Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="5e6e4-107">[إنشاء نهج نشاط تنبيه](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) لاستلام إشعارات عندما نقوم باكتشاف ملفات ضارة.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="5e6e4-108">للحصول على تعليمات كاملة، راجع هذا [الموضوع](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5e6e4-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="5e6e4-109">**ملاحظة**: حسب التصميم لا ATP فحص كل ملف واحد في SharePoint على الإنترنت، أندريف للعمل، أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="5e6e4-110">يتم تفحص الملفات بشكل غير متزامن بعملية تستخدم نشاط المشاركة، نشاط الضيف، وإشارات التهديد للتعرف على الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="5e6e4-111">لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5e6e4-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
