---
title: إصلاح تطبيقات Office حسابك في رسالة حالة سيئة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969187"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a>إصلاح تطبيقات Office "حسابك في حالة سيئة" خطأ

لإصلاح هذا الخطأ، حاول الخيارات التالية على الكمبيوتر المتأثر:

- فتح تطبيق Office، حدد تسجيل خروج**حساب** >  **الملف** > **من جميع الحسابات**. تسجيل الدخول مرة أخرى باستخدام حساب مستخدم بترخيص صالح. للحصول على معلومات تفصيلية، راجع [الحسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).
- [مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.<br>
  **ملاحظة:** تغيرت مسارات التسجيل لـ Office 2016 إلى 16.0. على سبيل المثال، \Software\Microsoft\Office\16.0\Common\Identity\
- على الكمبيوتر المتأثر، قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:  
     1. انقر بزر Windows وحدد **تشغيل**. في المربع **المفتوح،** اكتب **regedit**، ثم حدد **موافق**.
     2. حدد **نعم** عند المطالبة للسماح لمحرر التسجيل بإجراء تغييرات على جهازك.
    3. في محرر التسجيل، قم بإضافة قيمة DWORD من EnableADAL مع إعداد 0 تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.
- إذا حدث الخطأ أثناء الاتصال بـ Office 365 باستخدام Office 2013، [قم بتمكين المصادقة الحديثة](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) لعميل Office.

لمزيد من المعلومات، راجع [كيفية استكشاف الأخطاء وإصلاحها للتطبيقات غير المستعرض التي لا يمكنها تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).

