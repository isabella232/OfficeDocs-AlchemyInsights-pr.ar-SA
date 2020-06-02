---
title: ATP لSharePoint، OneDrive، وفرق مايكروسوفت
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: e9437d04815d4ca2f55cf9133ef6a4b429cd2476
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508399"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="23208-102">ATP لSharePoint، OneDrive، وفرق مايكروسوفت</span><span class="sxs-lookup"><span data-stu-id="23208-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="23208-103">اتبع الخطوات التالية لتمكين الحماية المتقدمة من التهديدات:</span><span class="sxs-lookup"><span data-stu-id="23208-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="23208-104">انتقل إلى [https://protection.office.com](https://protection.office.com) حساب مسؤول عمومي أو مسؤول أمان وسجّل الدخول إليه.</span><span class="sxs-lookup"><span data-stu-id="23208-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="23208-105">في جزء التنقل الأيسر تحت **إدارة التهديد،** اختر **Policy** \> **المرفقات الآمنة**للنهج.</span><span class="sxs-lookup"><span data-stu-id="23208-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="23208-106">حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="23208-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="23208-107">[إنشاء نهج تنبيه نشاط](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) لتلقي الإشعارات عندما نكتشف الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="23208-107">[Create an activity alert policy](https://docs.microsoft.com/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="23208-108">للحصول على إرشادات كاملة، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="23208-108">For complete instructions, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="23208-109">**ملاحظة:** حسب التصميم، لا تقوم ATP بمسح كل ملف في SharePoint Online أو OneDrive للأعمال أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="23208-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="23208-110">يتم مسح الملفات ضوئيًا بشكل غير متزامن بواسطة عملية تستخدم نشاط المشاركة ونشاط الضيف وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="23208-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="23208-111">لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="23208-111">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
