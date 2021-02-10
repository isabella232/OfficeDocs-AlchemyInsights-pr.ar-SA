---
title: مشكلة في مجموعات الأمان
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
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177353"
---
# <a name="issue-with-security-groups"></a>مشكلة في مجموعات الأمان

**إذا كنت تحصل على خطأ في الشبكة AADDS104**

قواعد مجموعة أمان الشبكة غير الصالحة هي السبب الأكثر شيوعا لأخطاء الشبكة لخدمات مجال Azure Active Directory (AD DS). يجب أن تسمح مجموعة أمان الشبكة للشبكة الظاهرية بالوصول إلى منافذ بروتوكولات وبروتوكولات معينة. إذا تم حظر هذه المنافذ، لا يمكن ل Azure مراقبة المجال المدار أو تحديثه. كما تؤثر المزامنة بين Azure AD و Azure AD DS. تأكد من الاحتفاظ بالمنافذ الافتراضية مفتوحة لتجنب انقطاع الخدمة.

لفهم التنبيهات الشائعة لحل مشاكل تكوين مجموعة أمان الشبكة، راجع [إضافة مجموعات الأمان والتحقق منها.](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)
