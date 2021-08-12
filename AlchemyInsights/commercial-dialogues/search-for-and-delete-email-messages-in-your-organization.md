---
title: البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948870"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك

اتبع الخطوات التالية:

1. إذا لم تكن المسؤول العام، للبحث عن الرسائل، يجب إضافة حسابك إلى مجموعة دور **eDiscovery Manager** أو دور إدارة البحث **في التوافق**. لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة دور **إدارة** المؤسسة أو دور إدارة البحث **واحذف**. يتم تعيين الأذونات لهذه الأدوار في مركز [& الأمان.](https://protection.office.com)
2. [قم بإنشاء بحث في المحتوى](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور على الرسالة التي تريد حذفها.
3. [الاتصال إلى الأمان & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). إذا كنت تستخدم المصادقة متعددة العوامل، فشاهد هذه الإرشادات: الاتصال إلى مركز التوافق & [PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) باستخدام المصادقة متعددة العوامل
4. حذف الرسالة: قم بتشغيل `New-ComplianceSearchAction` الأمر cmdlet لحذف الرسالة. يتم نقل الرسائل المحذوفة إلى مجلد العناصر القابلة لاسترداد المستخدم. للحصول على أمر مثال، راجع [الخطوة 3: حذف الرسالة.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
