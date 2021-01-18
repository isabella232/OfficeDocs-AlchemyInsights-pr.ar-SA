---
title: تكوين خدمه المجالات
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884806"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>تعذر تمكين AAD أو فشل النشر

لحل مشكله خدمه مجال Azure AD (AAD-DS) غير ممكنة أو فشل نشرها ، قم بتنفيذ الخطوات التالية:

1. إذا كنت تستخدم شبكه ظاهريه موجودة بالفعل ، فتحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة للمزامنة في AAD في المدخل https://aka.ms/aadds-networking .
2. تحقق لمعرفه ما إذا تم الرد علي رسالة الخطا الخاصة بك في دليل استكشاف الأخطاء وإصلاحها المتوفر في  https://aka.ms/aadds-troubleshoot-enable .
3. جرب نشر خدمات مجالات Azure AD في شبكه ظاهريه جديده.
4. اتبع دليل بدء الاستخدام حول كيفيه نشر AAD-DS: [إنشاء خدمات مجال AAD وتكوينها](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).
5. إذا واجهتك مشاكل في نشر خدمات مجالات Azure AD ، فراجع [استكشاف أخطاء خدمات مجال AZURE ad وإصلاحها](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) 

**تعذر تعطيل AAD-DS**

تعذر إيقاف AAD-DS مؤقتا. إذا كنت ترغب في التوقف عن استخدام مجالك المدار ، فيجب حذفه.
لحذف مجالك المدار ، راجع [حذف خدمه مجال AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).



