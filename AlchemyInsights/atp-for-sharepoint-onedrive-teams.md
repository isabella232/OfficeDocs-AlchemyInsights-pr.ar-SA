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
ms.openlocfilehash: 28046c61e1aedbb2c07cca3fc01b118d0dc3c143
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43712445"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="5b967-102">ATP لSharePoint، OneDrive، وفرق مايكروسوفت</span><span class="sxs-lookup"><span data-stu-id="5b967-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="5b967-103">اتبع الخطوات التالية لتمكين الحماية المتقدمة من التهديدات:</span><span class="sxs-lookup"><span data-stu-id="5b967-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="5b967-104">انتقل [https://protection.office.com](https://protection.office.com) إلى حساب مسؤول عمومي أو مسؤول أمان وسجّل الدخول إليه.</span><span class="sxs-lookup"><span data-stu-id="5b967-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="5b967-105">في جزء التنقل الأيسر تحت **إدارة التهديد،** اختر **المرفقات الآمنة** **للنهج.** \></span><span class="sxs-lookup"><span data-stu-id="5b967-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="5b967-106">حدد **تشغيل ATP لـ SharePoint و OneDrive وفرق Microsoft**.</span><span class="sxs-lookup"><span data-stu-id="5b967-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="5b967-107">[إنشاء نهج تنبيه نشاط](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) لتلقي الإشعارات عندما نكتشف الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="5b967-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="5b967-108">للحصول على إرشادات كاملة، راجع هذا [الموضوع](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5b967-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="5b967-109">**ملاحظة:** حسب التصميم، لا تقوم ATP بمسح كل ملف في SharePoint Online أو OneDrive للأعمال أو فرق Microsoft.</span><span class="sxs-lookup"><span data-stu-id="5b967-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="5b967-110">يتم مسح الملفات ضوئيًا بشكل غير متزامن بواسطة عملية تستخدم نشاط المشاركة ونشاط الضيف وإشارات التهديد لتحديد الملفات الضارة.</span><span class="sxs-lookup"><span data-stu-id="5b967-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="5b967-111">لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="5b967-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
