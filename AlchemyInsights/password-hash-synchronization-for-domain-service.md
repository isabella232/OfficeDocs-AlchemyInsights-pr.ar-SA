---
title: مزامنة كلمة المرور المتزامنة لخدمة المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8248"
- "9004400"
- "8249"
- "9003245"
ms.openlocfilehash: 7f138837b720926c5b687285a105eb0417ca5b39
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177352"
---
# <a name="password-hash-synchronization-for-domain-service"></a>مزامنة كلمة المرور المتزامنة لخدمة المجال

**إذا كان مثيل Azure AD DS يطالبك بتمكين مزامنة كلمة المرور**

تواجه سيناريو تقوم فيه بتشغيل بيئة مختلطة مع مزامنة المستخدمين من بيئة Azure Active Directory Domain Services (AD DS) المحلية. يتم مواجهة هذا السيناريو على الرغم من مزامنة كلمة المرور المتزامنة بين AD DS ومستأجر Azure AD.

**السبب**

يحدث هذا الأمر لأن Azure AD Connect لا يقوم بشكل افتراضي بمزامنة كلمات مرور Azure AD DS القديمة في New Technology Manager (NTLM) وKerberos.

**الحل البديل** 

قد تحتاج إلى تكوين Azure AD Connect لمزامنة كلمات المرور المتزامنة المطلوبة لمصادقة NTLM وKerberos.

بعد تكوين Azure AD Connect، يتزامن أيضا حدث إنشاء حساب أو تغيير كلمة مرور في الموقع مع Azure AD. الرجاء الاطلاع [هنا](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-password-hash-sync) للحصول على مزيد من المعلومات حول ذلك للحصول على إرشادات حول كيفية تمكين مزامنة كلمة المرور في بيئات Azure AD DS المختلطة.