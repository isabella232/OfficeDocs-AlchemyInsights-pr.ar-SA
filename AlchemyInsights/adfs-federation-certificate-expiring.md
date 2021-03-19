---
title: انتهت صلاحية شهادة اتحاد ADFS
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: a3172bc402a22999a3bf963233cc26db1ddf2a03
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686701"
---
# <a name="adfs-federation-certificate-expiring"></a>انتهت صلاحية شهادة اتحاد ADFS

لحل هذه المشكلة، اتبع الخطوات التالية:
  
1. ثبت وحدة Microsoft Azure Active Directory النمطية ل Windows PowerShell على الكمبيوتر (إذا لم تكن الوحدة النمطية مثبتة بالفعل). للقيام بذلك، انتقل إلى [إدارة Azure AD باستخدام Windows PowerShell](https://aka.ms/aadposh).

2. اتبع الخطوات في القسم "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز ل AD FS" من الخطأ "كان هناك مشكلة في الوصول إلى الموقع" من AD FS عند تسجيل مستخدم مقسم إلى [Microsoft 365](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)أو Azure أو Intune .

3. اتبع الخطوات في تحديث إعدادات مجال أو إصلاحها في Microsoft أو [Azure أو Intune](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365).

    لمعرفة المزيد حول تجديد شهادات الاتحاد، راجع تجديد شهادات الاتحاد ل [Microsoft 365 و Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
