---
title: الاتحاد ADFS انتهاء مدة صلاحية الشهادة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 518261787b1b0df99ee7b3dc3e51dec70e4373bc
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32398327"
---
# <a name="adfs-federation-certificate-expiring"></a>الاتحاد ADFS انتهاء مدة صلاحية الشهادة

لحل هذه المشكلة، اتبع الخطوات التالية:
  
1. تثبيت في Microsoft Azure نشط الدليل الوحدة النمطية ل Windows PowerShell على الكمبيوتر (إذا لم يتم تثبيت الوحدة النمطية مسبقاً). للقيام بذلك، انتقل إلى [إدارة استخدام Windows PowerShell الإعلان Azure](https://aka.ms/aadposh).
    
2. اتبع الخطوات الموجودة في "السيناريو 1: مدة صلاحية شهادة التوقيع الرمز المميز AD FS" المقطع ["كان هناك مشكلة في الوصول إلى الموقع" خطأ من خ الإعلان عند تسجيل مستخدم متحد Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).
    
3. اتبع الخطوات في [كيفية تحديث أو إصلاح إعدادات المجال المتحد في Office 365، الأزرق السماوي، أو إينتوني](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).
    
    لمزيد من المعلومات حول تجديد الشهادات الاتحاد، راجع [تجديد شهادات الاتحاد Office 365 و Active Directory Azure](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).
    

