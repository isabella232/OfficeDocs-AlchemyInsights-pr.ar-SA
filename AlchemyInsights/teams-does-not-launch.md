---
title: Teams تشغيل
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/4/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12673"
- "9007646"
ms.openlocfilehash: a37f980e700090da8199c703216af6f04f4aca464c21870beb3e907dd7b2d491
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57813340"
---
# <a name="teams-doesnt-launch"></a>Teams تشغيل

إذا حاولت فتح Microsoft Teams ولكن لم يتم تشغيلها مطلقا، فجرب ما يلي:

1. استعرض إلى **٪appdata٪\Microsoft\Teams**.
1. احذف محتويات المجلد.
1. أعد تشغيل الكمبيوتر، وحاول تشغيل Teams.

قد تحتاج إلى إعادة تثبيت Teams. لإعادة التثبيت:

1. إلغاء تثبيت Teams باستخدام لوحة التحكم.
1. استعرض إلى **٪appdata٪\Microsoft\Teams\ذاكرة التخزين المؤقت للتطبيق.**
1. احذف محتويات المجلد.
1. استعرض إلى **٪appdata٪\Microsoft\teams\ذاكرة التخزين المؤقت**.
1. احذف محتويات المجلد.
1. أعد تشغيل الكمبيوتر، ثم قم بتنزيل الكمبيوتر وتثبيته Teams.

إذا كنت تريد تشغيل تشخيص على المستأجر لمستخدم معين لا يمكنه تسجيل الدخول، فابدأ عملية بحث جديدة باستخدام الكلمة الأساسية **TeamsUserUnableToSignIn** واتبع المطالبات.