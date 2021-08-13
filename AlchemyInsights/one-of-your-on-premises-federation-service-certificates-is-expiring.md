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
ms.openlocfilehash: d0658b05b81ac45e7ce80323ad29898599482c4d3430d886627af6e9f8d136f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53985204"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>انتهت صلاحية إحدى شهادات خدمة الاتحاد المحلي

لحل هذه المشكلة، اتبع الخطوات التالية:
  
- قم بتثبيت Microsoft Azure Active Directory النمطية Windows PowerShell على الكمبيوتر (إذا لم تكن الوحدة النمطية مثبتة بالفعل). للقيام بذلك، انتقل إلى [Azure Active Directory PowerShell Graph](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- اتبع الخطوات في المقطع "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز ل AD FS" من الخطأ "كان هناك مشكلة في الوصول إلى الموقع" من [AD FS](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)عند تسجيل مستخدم مقسم إلى Microsoft 365 أو Azure أو Intune .
    
- اتبع الخطوات في كيفية تحديث إعدادات المجال المتحدة أو إصلاحها في Microsoft 365 أو [Azure أو Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع تجديد الشهادات ل [O365 و Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

