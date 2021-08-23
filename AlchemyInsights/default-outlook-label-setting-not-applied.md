---
title: إعداد Outlook الافتراضي غير مطبق
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000181"
- "13259"
ms.openlocfilehash: 84284554151586ff0a22f983d9494f59b4675f92
ms.sourcegitcommit: 4b92c2648ddba3ad3bc61a22771c59ed5fc76303
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/17/2021
ms.locfileid: "58454406"
---
# <a name="default-outlook-label-setting-not-applied"></a>إعداد Outlook الافتراضي غير مطبق

إذا لم يتم تطبيق إعدادات التسمية الافتراضية Outlook بشكل صحيح ولم يتم تطبيق تسمية مختلفة أو لم يتم تطبيق أي تسمية، فمن الممكن أن تواجه مشكلة معروفة (MC277818) ويجب أن تقوم بأي من هذين الخيارين لحل المشكلة:

**الخيار 1:**

1. انتقل إلى Microsoft 365 التوافق > حماية   >  **معلومات الحلول.**
1. حدد **نهج التسمية**، وحدد نهج التسمية الذي تحتاج إلى تحريره ( لم يتم تعيين إعداد **OutlookDefaultlabel** بشكل صحيح على نهج التسمية المعني. قم **بتشغيل Get-labelpolicy** لعرض هذا الإعداد)، ثم حدد **تحرير النهج**.
1. حدد **التالي** حتى ترى الإعداد تطبيق هذه التسمية الافتراضية على  رسائل البريد **الإلكتروني،** التي تتوفر إذا حددت طلب  من المستخدمين تطبيق تسمية على رسائل البريد الإلكتروني والمستندات الخاصة بالوريث في مربع الحوار إعدادات النهج.
1. في **مربع الحوار تطبيق تسمية افتراضية** على المستندات، اختر **بلا** من القائمة المنسدلة.
1. حدد  التالي **وإرسال** لحفظ إعدادات التسمية.

**الخيار 2:**

في مركز الأمان والتوافق [Powershell](https://docs.microsoft.com/powershell/exchange/connect-to-scc-powershell?view=exchange-ps)، استخدم الأمر Set-LabelPolicy لتغيير **OutlookDefaultlabel** إلى **بلا** على {OutlookDefaultLabel="None"}.

تشغيل: `Set-LabelPolicy -Identity [policy] -AdvancedSettings @{OutlookDefaultLabel="None"}`

لمزيد من المعلومات حول التسميات الافتراضية Outlook، راجع تعيين تسمية افتراضية مختلفة [Outlook](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide-customizations#set-a-different-default-label-for-outlook).