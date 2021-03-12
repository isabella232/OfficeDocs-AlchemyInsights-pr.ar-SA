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
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743156"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>البحث عن رسائل البريد الإلكتروني وحذفها في مؤسستك

اتبع الخطوات التالية:

1. إذا لم تكن المسؤول العام، للبحث عن الرسائل، يجب إضافة حسابك إلى مجموعة دور **eDiscovery Manager** أو دور إدارة البحث **في التوافق**. لحذف الرسائل، ستحتاج إلى الانضمام إلى مجموعة دور **إدارة** المؤسسة أو دور إدارة البحث **واحذف**. يتم تعيين الأذونات لهذه الأدوار في مركز [& الأمان.](https://protection.office.com)
2. [قم بإنشاء بحث في المحتوى](https://docs.microsoft.com/office365/securitycompliance/content-search) للعثور على الرسالة التي تريد حذفها.
3. [الاتصال بمركز & التوافق PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell). إذا كنت تستخدم المصادقة متعددة العوامل، فشاهد هذه الإرشادات: الاتصال بمركز التوافق & [PowerShell باستخدام](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell) المصادقة متعددة العوامل
4. حذف الرسالة: قم بتشغيل `New-ComplianceSearchAction` الأمر cmdlet لحذف الرسالة. يتم نقل الرسائل المحذوفة إلى مجلد العناصر القابلة لاسترداد المستخدم. للحصول على أمر مثال، راجع [الخطوة 3: حذف الرسالة.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)
