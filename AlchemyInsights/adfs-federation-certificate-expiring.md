---
title: انتهاء صلاحيه شهادة الاتحاد ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: eafd31e91340b41b7948fb1fe62889731b816d9a
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36737176"
---
# <a name="adfs-federation-certificate-expiring"></a>انتهاء صلاحيه شهادة الاتحاد ADFS

لحل هذه المشكلة ، اتبع الخطوات التالية:
  
1. تثبيت Microsoft Azure Active Directory الوحدة النمطية ل Windows PowerShell علي الكمبيوتر (إذا لم تكن الوحدة النمطية مثبته بالفعل). للقيام بذلك ، انتقل إلى [أداره الإعلان Azure باستخدام Windows PowerShell](https://aka.ms/aadposh).

2. اتبع الخطوات الموجودة في "السيناريو 1: انتهت صلاحيه شهادة توقيع الرمز المميز AD FS" المقطع من ["كان هناك مشكله في الوصول إلى الموقع" خطا من AD FS عندما يقوم مستخدم متحد بتسجيل الدخول إلى Office 365 أو Azure اينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. اتبع الخطوات التالية في [تحديث أو إصلاح إعدادات مجال المتحدة في Office 365 أو Azure اينتوني](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    لمزيد من المعلومات حول تجديد شهادات الاتحاد ، راجع [تجديد شهادات الاتحاد ل Office 365 والدليل النشط Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
