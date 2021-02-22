---
title: إخفاء المجلدات العامة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/18/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "8417"
ms.openlocfilehash: 70179296e9c1bb7391535f55796bc5af80b825f8
ms.sourcegitcommit: a019bd8b0244914edb59e124bc6538cdc5c158f9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/18/2021
ms.locfileid: "50315307"
---
# <a name="hide-public-folders"></a>إخفاء المجلدات العامة

**لإخفاء شجرة المجلدات العامة بالكامل:**

استخدم الخطوات في [هذه](https://aka.ms/ControlPF) المقالة لإخفاء شجرة المجلدات العامة بالكامل عن المحدد أو جميع المستخدمين.

**لإخفاء مجلد عمومي معين:**

1. إضافة أذونات للمستخدمين الذين يحتاجون إلى الوصول إلى المجلد العمومي

    `Add-PublicFolderClientPermission \test1 -User cloud1 -AccessRights owner`

2. إزالة المستخدم **الافتراضي** من **قائمة الأذونات:**

    `Remove-PublicFolderClientPermission \test1 -User Default`
