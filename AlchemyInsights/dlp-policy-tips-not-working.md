---
title: تلميحات نهج DLP لا تعمل
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 8a3b8175c077b77d1c9b5d859012faddcb1fa3a0
ms.sourcegitcommit: 099704f7f4bdf122d09bb4f7cc71d36fc77a7fcf
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2021
ms.locfileid: "51958689"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="4404a-102">مشاكل تلميح نهج DLP</span><span class="sxs-lookup"><span data-stu-id="4404a-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="4404a-103">**هام**: خلال هذه الأوقات غير المسبوقة، نقوم باتخاذ الخطوات اللازمة لضمان توفر خدمات SharePoint Online و OneDrive بشكل كبير – الرجاء زيارة [تعديلات الميزات المؤقتة لـ SharePoint Online](https://aka.ms/ODSPAdjustments) للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="4404a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="4404a-104">لتكوين تلميحات النهج حول نهج DLP في مركز & الأمان والتوافق في وضع التنفيذ الكامل، قم بما يلي:</span><span class="sxs-lookup"><span data-stu-id="4404a-104">To configure policy tips on your DLP policy in the Security & Compliance center in full enforcement mode, do the following:</span></span>

- <span data-ttu-id="4404a-105">تأكد من تمكين تلميحات **النهج** على قاعدة DLP.</span><span class="sxs-lookup"><span data-stu-id="4404a-105">Ensure policy tips have been **enabled** on the DLP rule.</span></span> <span data-ttu-id="4404a-106">للحصول على الخطوات، راجع [إرسال إعلامات البريد الإلكتروني وإظهار تلميحات النهج لنهج DLP](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="4404a-106">For steps, see [Send email notifications and show policy tips for DLP policies](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="4404a-107">تأكد من تطابق المحتوى مع ما هو مطلوب لتحريك القاعدة الموضحة في تعريفات كيان نوع المعلومات [الحساسة](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="4404a-107">Ensure your content matches what is required to trigger the rule outlined in [Sensitive information type entity definitions](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="4404a-108">يتم عرض تلميحات النهج في كل من OWA و Outlook.</span><span class="sxs-lookup"><span data-stu-id="4404a-108">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="4404a-109">ومع ذلك، عند استخدام Outlook 2013 أو أي وقت لاحق، يتم عرض تلميحات النهج فقط في ظروف معينة.</span><span class="sxs-lookup"><span data-stu-id="4404a-109">However, when using Outlook 2013 or later, policy tips are displayed only under certain conditions.</span></span> <span data-ttu-id="4404a-110">للحصول على قائمة الشروط المحددة، راجع الشروط المعتمدة ل [Outlook 2013](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)أو أي وقت لاحق لعرض تلميحات النهج .</span><span class="sxs-lookup"><span data-stu-id="4404a-110">For the specific conditions list, see [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips).</span></span>

<span data-ttu-id="4404a-111">للحصول على معلومات حول تلميحات نهج DLP، راجع مرجع تلميحات نهج [DLP](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) ومصفوفة الدعم [لتلميحات نهج DLP](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span><span class="sxs-lookup"><span data-stu-id="4404a-111">For information on DLP Policy tips, see [DLP Policy Tips Reference](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps) and [Support Matrix for DLP Policy tips](https://docs.microsoft.com/microsoft-365/compliance/dlp-policy-tips-reference?view=o365-worldwide#support-matrix-for-dlp-policy-tips-across-microsoft-apps).</span></span>