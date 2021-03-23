---
title: تكوين نقطة اتصال الخدمة (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034795"
---
# <a name="configure-service-connection-point-scp"></a>تكوين نقطة اتصال الخدمة (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **السبب**: يتعذر قراءة كائن SCP والحصول على معلومات مستأجر Azure AD
- **الدقة**: الرجوع إلى المقطع [تكوين نقطة اتصال الخدمة](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**خطة الإجراء**

- تحقق مما إذا كان الجهاز قد استلم "GPO" للتحقق من الصحة الذي تم التحكم به.
- تأكد من أن مكتب GPO قد أنشأ مفاتيح التسجيل.
- تأكد من أن لديك مفتاحين تم إنشاؤهما باستخدام مجال Onmicrosoft وم ID الدليل.

**تكوين إعداد التسجيل من جانب العميل ل SCP**

استخدم المثال التالي لإنشاء كائن نهج المجموعة (GPO) لنشر إعداد تسجيل ينشئ إدخال SCP في سجل أجهزتك.

1. افتح وحدة تحكم "إدارة نهج المجموعة" وأنشئ "نهج نهج المجموعة" جديدا في مجالك.
     - قم بتوفير اسم ل GPO الذي تم إنشاؤه حديثا (على سبيل المثال، ClientSideSCP)

2. قم بتحرير GPO وحدد موقع المسار التالي: تكوين الكمبيوتر > التفضيلات > **Windows > السجل.**

3. انقر بضغطة زر الماوس **الأيمن فوق التسجيل** وحدد عنصر > السجل **الجديد.**

4. على علامة **التبويب عام،** قم بتكوين ما يلي:
  
- **الإجراء**: تحديث
    
- **الخلية**: HKEY_LOCAL_MACHINE
    
- **مسار المفتاح**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **اسم القيمة**: TenantId
    
- **نوع القيمة**: REG_SZ
    
- **بيانات القيمة**: المثيل GUID أو الدليل لمثيل Azure AD (يمكن العثور على هذه القيمة في مدخل **Azure > Azure Active Directory > Properties > الدليل**)
 
- انقر فوق **موافق**.
 
5. انقر بضغطة زر الماوس **الأيمن فوق التسجيل** وحدد عنصر > السجل **الجديد.**

6. على علامة **التبويب عام،** قم بتكوين ما يلي:
  
- **الإجراء**: تحديث
    
- **الخلية**: HKEY_LOCAL_MACHINE
    
- **مسار المفتاح**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **اسم القيمة**: TenantName
    
- **نوع القيمة**: REG_SZ
    
- **بيانات القيمة**: اسم المجال الذي تم التحقق منه إذا كنت تستخدم بيئة متكاتف مثل AD FS. اسم المجال المتحقق منه أو اسم مجالك onmicrosoft.com (على سبيل المثال، contoso.onmicrosoft).com إذا كنت تستخدم بيئة مدارة

- انقر فوق **موافق**.

7. أغلق محرر GPO الذي تم إنشاؤه حديثا.

8. ربط "مجموعة معلومات المجموعة" التي تم إنشاؤها حديثا ب OU المطلوب الذي يحتوي على أجهزة الكمبيوتر المنضمة إلى المجال والتي تنتمي إلى عدد السكان الذي تم التحكم في طرحه.

لمزيد من المعلومات، راجع التحقق من الصحة المتحكم به لضم [Azure AD المختلط - Azure AD | أجهزة Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) وإصلاحها المختلطة  [التي انضم إليها Azure Active Directory | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









