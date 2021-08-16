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
ms.openlocfilehash: 101c0ba90d2bec6b1684fd63645ba2f8f89783ad5bfdf0efe739d31dfd951f66
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044399"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint

إذا كنت تتلقى الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint فقد يكون مرتبطا ب إهمال TLS 1.0/1.1. لمزيد من المعلومات، راجع المقالات التالية:

- [التحضير ل TLS 1.2 في Office 365 Office 365 سحابة القطاع الحكومي](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [تحدث أخطاء المصادقة إذا لم يكن لدى العميل دعم TLS 1.2](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [تحديث لتمكين TLS 1.1 و TLS 1.2 كبروتوكولات آمنة افتراضية في WinHTTP في Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

إذا كان المستخدمون Windows 7، فتأكد من التحقق من [مجموعات TLS Cipher في](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .