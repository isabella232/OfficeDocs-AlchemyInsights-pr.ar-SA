---
title: مشاكل تتعلق SharePoint على Windows 7 أجهزة
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/28/2021
ms.locfileid: "52124750"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a><span data-ttu-id="ca02c-102">مشاكل تتعلق SharePoint على Windows 7 أجهزة</span><span class="sxs-lookup"><span data-stu-id="ca02c-102">Issues with SharePoint on Windows 7 machines</span></span>

<span data-ttu-id="ca02c-103">إذا تلقيت أخطاء على أجهزة Windows 7 أثناء العمل على SharePoint أو OneDrive، فقد تكون مرتبطة ب إهمال TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="ca02c-103">If you receive errors on Windows 7 machines while working on SharePoint or OneDrive, they might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="ca02c-104">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="ca02c-104">For more information, see:</span></span>

- [<span data-ttu-id="ca02c-105">التحضير ل TLS 1.2 في Office 365 Office 365 سحابة القطاع الحكومي</span><span class="sxs-lookup"><span data-stu-id="ca02c-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- <span data-ttu-id="ca02c-106">Windows 7 SP1/Windows 8 تمكين TLS1.2 لعملاء العملاء.</span><span class="sxs-lookup"><span data-stu-id="ca02c-106">Windows 7 SP1/Windows 8 clients must have TLS1.2 enabled.</span></span> <span data-ttu-id="ca02c-107">لمزيد من المعلومات، راجع حدوث أخطاء المصادقة عندما لا يكون لدى العميل [دعم TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span><span class="sxs-lookup"><span data-stu-id="ca02c-107">For more information, see [Authentication errors occur when client doesn't have TLS 1.2 support](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)</span></span>

- <span data-ttu-id="ca02c-108">ثبت KB3140245 وأنشئ قيمة السجل.</span><span class="sxs-lookup"><span data-stu-id="ca02c-108">Install KB3140245 and create the registry value.</span></span> <span data-ttu-id="ca02c-109">لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) كبروتوكولات آمنة افتراضية في WinHTTP في Windows</span><span class="sxs-lookup"><span data-stu-id="ca02c-109">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)</span></span>

- <span data-ttu-id="ca02c-110">Windows 7 SP1/Windows 8 التأكد من تثبيت أحدث مجموعات رموز TLS.</span><span class="sxs-lookup"><span data-stu-id="ca02c-110">Windows 7 SP1/Windows 8 clients must ensure latest TLS cipher suites are installed.</span></span> <span data-ttu-id="ca02c-111">لمزيد من المعلومات، راجع [3042058 مستشار أمان Microsoft](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span><span class="sxs-lookup"><span data-stu-id="ca02c-111">For more information, see [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058).</span></span> 


