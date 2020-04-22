---
title: تنتهي صلاحية إحدى شهادات خدمة الاتحاد المحلي
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 172084b7-68a1-42a5-944d-2e871eaa2972
ms.openlocfilehash: 24c369c61ad7cf7a9fe101ac29271c32e5159c1f
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43761370"
---
# <a name="one-of-your-on-premises-federation-service-certificates-is-expiring"></a>تنتهي صلاحية إحدى شهادات خدمة الاتحاد المحلي

لحل هذه المشكلة، اتبع الخطوات التالية:
  
- قم بتثبيت وحدة الدليل النشط من Microsoft Azure لـ Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية بالفعل). للقيام بذلك، انتقل إلى [Azure Active Directory PowerShell للرسم البياني](https://docs.microsoft.com/powershell/azure/active-directory/install-adv2?view=azureadps-2.0)
    
- اتبع الخطوات في المقطع "السيناريو 1: انتهت صلاحية شهادة توقيع الرمز المميز AD FS" من [خطأ "كانت هناك مشكلة في الوصول إلى الموقع" من AD FS عندما يسجل مستخدم موحد الدخول إلى Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
- اتبع الخطوات في ر[كيفية تحديث أو إصلاح إعدادات مجال موحد في Office 365 أو Azure أو Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
لمزيد من المعلومات حول تجديد شهادات الاتحاد، راجع [تجديد الشهادة لـ O365 و Azure AD](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
  

