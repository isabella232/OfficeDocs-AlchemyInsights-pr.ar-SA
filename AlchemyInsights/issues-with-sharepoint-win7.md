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
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>مشاكل تتعلق SharePoint على Windows 7 أجهزة

إذا تلقيت أخطاء على أجهزة Windows 7 أثناء العمل على SharePoint أو OneDrive، فقد تكون مرتبطة ب إهمال TLS 1.0/1.1. لمزيد من المعلومات، اطلع على:

- [التحضير ل TLS 1.2 في Office 365 Office 365 سحابة القطاع الحكومي](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 تمكين TLS1.2 لعملاء العملاء. لمزيد من المعلومات، راجع حدوث أخطاء المصادقة عندما لا يكون لدى العميل [دعم TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- ثبت KB3140245 وأنشئ قيمة السجل. لمزيد من المعلومات، راجع التحديث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392) كبروتوكولات آمنة افتراضية في WinHTTP في Windows

- Windows 7 SP1/Windows 8 التأكد من تثبيت أحدث مجموعات رموز TLS. لمزيد من المعلومات، راجع [3042058 مستشار أمان Microsoft](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


