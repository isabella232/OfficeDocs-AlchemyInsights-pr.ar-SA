---
title: تم إغلاق الاتصال الأساسي في SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233413"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint

إذا كنت تتلقى الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint فقد يكون مرتبطا ب إهمال TLS 1.0/1.1. لمزيد من المعلومات، راجع المقالات التالية:

- [التحضير ل TLS 1.2 في Office 365 Office 365 سحابة القطاع الحكومي](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [تحدث أخطاء المصادقة إذا لم يكن لدى العميل دعم TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

إذا كان المستخدمون Windows 7، فتأكد من التحقق من [مجموعات TLS Cipher في](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .