---
title: وحدة التحكم في المجال
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49900732"
---
# <a name="domain-controller"></a>وحدة التحكم في المجال

**تعذر تمكين AAD أو فشل النشر**

لحل مشكله خدمه مجال Azure AD (AAD-DS) غير ممكنة أو فشل نشرها ، قم بتنفيذ الخطوات التالية:

1. إذا كنت تستخدم شبكه ظاهريه موجودة بالفعل ، فتحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة للمزامنة في AAD في المدخل https://aka.ms/aadds-networking .
2. تحقق لمعرفه ما إذا تم الرد علي رسالة الخطا الخاصة بك في دليل استكشاف الأخطاء وإصلاحها المتوفر في  https://aka.ms/aadds-troubleshoot-enable .
3. جرب نشر خدمات مجالات Azure AD في شبكه ظاهريه جديده.
4. اتبع دليل بدء الاستخدام حول كيفيه نشر AAD-DS ، والمتوفرة في [البرنامج التعليمي لإنشاء خدمات مجال AZURE AD](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. إذا واجهتك مشاكل في نشر خدمات مجالات Azure AD ، فراجع [استكشاف أخطاء خدمات مجال AZURE ad وإصلاحها](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) 

**تعذر تعطيل AAD-DS**

تعذر إيقاف AAD-DS مؤقتا. إذا كنت ترغب في التوقف عن استخدام مجالك المدار ، فيجب حذفه.

إذا واجهت مشاكل ، لحل رسائل الخطا الشائعة والخطوات المتعلقة باستكشاف الأخطاء وإصلاحها لمساعدتك علي تنفيذ المهام مره أخرى ، راجع [استكشاف الأخطاء وإصلاحها ل Azure active Directory Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).
