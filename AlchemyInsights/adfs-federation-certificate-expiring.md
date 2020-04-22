---
title: شهادة اتحاد ADFS تنتهي صلاحيتها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 14e7da6220dfa96edca5d9ec5c32e003480a9eaf
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43710394"
---
# <a name="adfs-federation-certificate-expiring"></a>شهادة اتحاد ADFS تنتهي صلاحيتها

لحل هذه المشكلة، اتبع الخطوات التالية:
  
1. قم بتثبيت وحدة الدليل النشط من Microsoft Azure لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل). للقيام بذلك، انتقل إلى [إدارة Azure AD باستخدام Windows PowerShell](https://aka.ms/aadposh).

2. اتبع الخطوات في المقطع "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من ["كانت هناك مشكلة في الوصول إلى الموقع" من AD FS عندما يسجل مستخدم موحد الدخول إلى Microsoft 365 أو Azure أو Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).

3. اتبع الخطوات في [تحديث أو إصلاح إعدادات مجال موحد في Microsoft أو Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    لمعرفة المزيد حول تجديد شهادات الاتحاد، راجع [تجديد شهادات الاتحاد لـ Microsoft 365 وAzure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
