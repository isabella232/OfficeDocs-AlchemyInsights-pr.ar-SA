---
title: الوصول المشروط مع إينتوني
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: 2e778bf4fbdb766700fb24b3405b4ddce89253f7
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29935915"
---
# <a name="conditional-access-with-intune"></a>الوصول المشروط مع إينتوني

يتطلب استخدام **الوصول المشروط** مع إينتوني ثلاث خطوات: 
  
- إنشاء **نهج الوصول الشرطي** بتعريف الموارد التي يتم حمايتها، وما هي الشروط اللازم استيفاؤها للوصول إلى هذه الموارد. على سبيل المثال، جهاز يجب أن تكون متوافقة مع قبل الوصول إلى البريد الإلكتروني. 
    
- إنشاء **نهج التوافق** لتحديد الإعدادات التي يجب استيفاؤها قبل تعتبر متوافقة مع الجهاز. على سبيل المثال، يجب أن يكون جهاز pin على الأقل 6 أرقام قبل أن يعتبر متوافق. 
    
- ضمان **توافق السياسات** و **نهج الوصول الشرطي** تستهدف مجموعات المستخدمين المطلوب. قد يتطلب هذا إنشاء مجموعات معينة من المستخدمين في Active Directory Azure. 
    
مزيد من المعلومات:
  
- [أفضل ممارسات الوصول الشرطي](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [الشروع في العمل مع "الوصول المشروط"](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

