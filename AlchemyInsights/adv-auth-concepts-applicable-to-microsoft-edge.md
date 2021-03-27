---
title: مفاهيم المصادقة المتقدمة المطبقة على Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398536"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>مفاهيم المصادقة المتقدمة المطبقة على Microsoft Edge

فيما يلي مفاهيم المصادقة المتقدمة التي تنطبق على Microsoft Edge:

**المصادقة الاستباقية**

عند تمكين نهج [ProactiveAuthEnabled،](https://go.microsoft.com/fwlink/?linkid=2134621) سيحاول Microsoft Edge المصادقة بشكل استباقي على المستخدمين الذين تم توقيعهم من خلال خدمات Microsoft. في فواصل زمنية منتظمة، سيستخدم خدمة عبر الإنترنت للتحقق من وجود بيان محدث يحتوي على التكوين الذي يحكم المصادقة الاستباقية.

الفوائد: تمكن المصادقة الاستباقية المصادقة للخدمات الأساسية، مثل صفحة علامة تبويب Office الجديدة. بالإضافة إلى ذلك، إذا تم استخدام Bing كمحرك بحث، فإن المصادقة الاستباقية تحسن أداء شريط العنوان وتساعد على إنشاء نتائج بحث مخصصة لتلبية احتياجات عملك.

**Windows Hello CredUI لمصادقة NTLM**

إذا لم يكن تسجيل الدخول الفردي (SSO) متوفرا عندما يحاول موقع ويب تسجيل الدخول إلى المستخدم من خلال الآلية NTLM أو التفاوض، فإن هذه الميزة ستسمح للمستخدم بمشاركة بيانات اعتماد نظام التشغيل مع موقع ويب وتلبية تحدي المصادقة باستخدام واجهة مستخدم Windows Hello Cred. سيظهر تدفق تسجيل الدخول هذا فقط في Windows 10 فقط للمستخدمين الذين لم ينتهوا من تسجيل الدخول خلال NTLM أو في تحدي التفاوض.

**استخدام كلمات المرور المحفوظة في تسجيل الدخول تلقائيا**

يمكن للمستخدمين الذين يحفظون كلمات المرور في Microsoft Edge تمكين تسجيل الدخول التلقائي إلى مواقع الويب حيث تم حفظ بيانات الاعتماد. يمكن للمستخدمين تشغيل هذه الميزة أو إيقاف تشغيلها في edge://settings/passwords، كما يمكنك تكوينها في سياسات [إدارة كلمات](https://go.microsoft.com/fwlink/?linkid=2134622) المرور.
