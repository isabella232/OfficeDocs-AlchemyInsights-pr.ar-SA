---
title: إزالة خدمة الخلفية ل Microsoft Search في Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816058"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a>إزالة خدمة الخلفية ل Microsoft Search في Bing

لإزالة خدمة الخلفية ل Microsoft Search في Bing، يمكنك تجربة الحلول التالية:

1. لإعادة إعدادات محرك البحث الأصلي، يمكنك القيام بما يلي:

    أ. قم **بتبديل مفتاح التبديل [](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) استخدام Bing** كمحرك بحث افتراضي إلى إيقاف التشغيل .

    ب. [انتقل إلى مركز إدارة Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) ومسح الإعداد الذي يؤثر على جميع المستخدمين في مؤسستك.

2. لإزالة خدمة الخلفية من جهاز فردي، قم بالمهام التالية:

    أ. اختر **لوحة التحكم > البرامج > والبرامج والميزات**.

    ب. انقر ب زر **الماوس الأيمن فوق بحث Microsoft في Bing** ضمن قائمة البرامج المثبتة، ثم انقر فوق إلغاء **التثبيت.**

3. لإزالة خدمة الخلفية من أجهزة متعددة في مؤسستك، سجل دخولك كمسؤول ثم قم بتشغيل الأمر التالي في برنامج نصي: 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
