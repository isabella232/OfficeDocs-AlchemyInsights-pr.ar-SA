---
title: اختبار تكوين IRM لإمكانيات OME الجديدة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: 62697d6379ea6ab3c6af86d3bab752af560da7c1250e5ef6dd2a3eae8023a05e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "57812428"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>اختبار تكوين IRM لإمكانيات OME الجديدة

للتحقق من تكوين Microsoft 365 المستأجر لاستخدام قدرات OME الجديدة، قم بتشغيل cmdlets التالية أثناء الاتصال Exchange Online [PowerShell:](/powershell/exchange/exchange-online-powershell)


1. تحقق من تكوين IRM للمستأجر عن طريق تشغيل `Get-IRMConfiguration` . تأكد من تعيين هذه القيم إلى **True**:
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. باستخدام مجالك وعنوان المرسل والمستلم، قم بتشغيل `Test-IRMConfiguration` . إذا لم يجتاز الاختبار الاختبار، فتحقق من تكوين IRM.

لمزيد من المعلومات حول كيفية التحقق من تكوين IRM، راجع التحقق من تكوين [OME الجديد في Exchange Online PowerShell](/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell).