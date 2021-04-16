---
title: انتهت صلاحية إحدى شهادات خدمة الاتحاد المحلي
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 45a679e83aa8f07d65d2e7e84d7eb2a2b5a721e8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810039"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>انتهت صلاحية إحدى شهادات خدمة الاتحاد المحلي

لحل هذه المشكلة، اتبع الخطوات التالية:
  
- ثبت وحدة Microsoft Azure Active Directory النمطية ل Windows PowerShell على الكمبيوتر (إذا لم تكن الوحدة النمطية مثبتة بالفعل). للقيام بذلك، انتقل إلى [Azure Active Directory PowerShell ل Graph ](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- اتبع الخطوات في القسم "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز ل AD FS" من الخطأ "كان هناك مشكلة في الوصول إلى الموقع" من AD FS عند تسجيل مستخدم مقسم إلى [Microsoft 365](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)أو Azure أو Intune .
    
- اتبع الخطوات في كيفية تحديث إعدادات المجال المتحدة أو إصلاحها في [Microsoft 365 أو Azure أو Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع تجديد الشهادات ل [O365 و Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

