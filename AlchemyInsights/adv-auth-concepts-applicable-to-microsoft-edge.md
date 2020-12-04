---
title: مفاهيم المصادقة المتقدمة المطبقة علي Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573267"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>مفاهيم المصادقة المتقدمة المطبقة علي Microsoft Edge

فيما يلي مفاهيم المصادقة المتقدمة التي تنطبق علي Microsoft Edge:

**المصادقة الاستباقية**

عند تمكين نهج [برواكتيفيوثينابليد](https://go.microsoft.com/fwlink/?linkid=2134621) ، سيحاول Microsoft Edge مصادقه المستخدمين الذين تم تسجيل دخولهم بفاعليه عبر خدمات Microsoft. عند الفواصل الزمنيه المنتظمة ، ستستخدم خدمه عبر الإنترنت للتحقق من البيانات المحدثة التي تحتوي علي المصادقة الاستباقية لتحكم التكوين.

الفوائد: تمكن المصادقة الاستباقية المصادقة علي الخدمات الاساسيه ، مثل صفحه علامة التبويب الجديدة في Office. بالاضافه إلى ذلك ، إذا تم استخدام Bing كمحرك بحث ، فان المصادقة الاستباقية تحسن أداء شريط العناوين ويساعد علي إنشاء نتائج البحث المخصصة لاحتياجات شركتك.

**كريدوي Windows Hello لمصادقه NTLM**

إذا لم تكن ميزه تسجيل الدخول الأحادي (SSO) متوفرة عندما يحاول موقع ويب تسجيل الدخول علي المستخدم من خلال اليه NTLM أو التفاوض ، ستسمح هذه الخاصية للمستخدم بمشاركه بيانات اعتماد نظام التشغيل باستخدام موقع ويب ولتلبيه ارتياب المصادقة بواسطة واجهه مستخدم بيانات الاعتماد الخاصة ب Windows Hello. سيظهر تدفق تسجيل الدخول هذا فقط في Windows 10 وللمستخدمين الذين لا يمكنهم الحصول علي SSO خلال NTLM أو تحدي في التفاوض.

**استخدام كلمات المرور المحفوظة لتسجيل الدخول تلقائيا**

يمكن للمستخدمين الذين يحفظون كلمات المرور في Microsoft Edge تمكين تسجيل الدخول التلقائي إلى مواقع الويب التي قاموا بحفظ بيانات الاعتماد بها. يمكن للمستخدمين تشغيل هذه الميزة أو إيقاف تشغيلها في edge://settings/passwords ، ويمكنك تكوينها في نهج [أداره كلمه المرور](https://go.microsoft.com/fwlink/?linkid=2134622) .
