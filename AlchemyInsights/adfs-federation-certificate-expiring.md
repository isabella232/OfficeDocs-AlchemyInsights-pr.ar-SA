---
title: انتهاء صلاحية شهادة الاتحاد ADFS
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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737176"
---
# <a name="adfs-federation-certificate-expiring"></a>انتهاء صلاحية شهادة الاتحاد ADFS

لحل هذه المشكلة، اتبع الخطوات التالية:
  
1. تثبيت الوحدة النمطية لـ Microsoft Azure Active Directory لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل). للقيام بذلك، انتقل إلى [إدارة إعلان Azure باستخدام Windows PowerShell](https://aka.ms/aadposh).

2. اتبع الخطوات الموجودة في "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من ["كان هناك مشكلة في الوصول إلى الموقع" خطأ من AD FS عند تسجيل دخول مستخدم متحد إلى Office 365 أو Azure إينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. اتبع الخطوات الموجودة في [تحديث أو إصلاح إعدادات مجال متحد في Office 365 أو Azure أو إينتوني](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع [تجديد شهادات الاتحاد لOffice 365 و Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
