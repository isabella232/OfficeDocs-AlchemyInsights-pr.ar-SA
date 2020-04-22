---
title: الوصول المشروط مع Intune
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: c9c47d71b2da3840504d5b28c7c9e067b4c05fa5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706008"
---
# <a name="conditional-access-with-intune"></a>الوصول المشروط مع Intune

يتطلب استخدام **الوصول الشرطي** مع Intune 3 خطوات: 
  
- إنشاء **نهج الوصول المشروط** الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب الوفاء بها للوصول إلى تلك الموارد. على سبيل المثال، يجب أن يكون الجهاز متوافقًا قبل الوصول إلى البريد الإلكتروني للشركة. 
    
- إنشاء **نهج الامتثال** لتعريف الإعدادات التي يجب الوفاء بها قبل اعتبار الجهاز متوافقًا. على سبيل المثال، يجب أن يحتوي الجهاز على دبوس لا يقل عن 6 أرقام قبل اعتباره متوافقًا. 
    
- ضمان توجيه كل من **سياسات الامتثال** وسياسات الوصول **المشروط** إلى المجموعات المطلوبة من المستخدمين. قد يتطلب هذا إنشاء مجموعات معينة من المستخدمين في Azure Active Directory. 
    
اقرأ المزيد:
  
- [أفضل ممارسات الوصول المشروط](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [البدء باستخدام الوصول المشروط](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

