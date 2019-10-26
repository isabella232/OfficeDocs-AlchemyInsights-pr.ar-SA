---
title: الوصول المشروط مع اينتوني
ms.author: pebaum
author: pebaum
ms.date: 10/11/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: aecba7c5-e86d-4ec8-9d44-679f5a3d659d
ms.openlocfilehash: e147e7460ee6a786e577a43c0b8355fc27ee367b
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36504981"
---
# <a name="conditional-access-with-intune"></a>الوصول المشروط مع اينتوني

يتطلب استخدام **الوصول المشروط** مع اينتوني 3 خطوات: 
  
- إنشاء **نهج الوصول المشروط** الذي يحدد الموارد المحمية ، وما هي الشروط التي يجب تلبيتها للوصول إلى تلك الموارد. علي سبيل المثال ، يجب ان يكون الجهاز متوافقا قبل الوصول إلى البريد الكتروني للشركة. 
    
- إنشاء **نهج توافق** لتعريف الإعدادات التي يجب ان تتحقق قبل اعتبار الجهاز متوافقا. علي سبيل المثال ، يجب ان يكون للجهاز دبوس بسته أرقام علي الأقل قبل اعتباره متوافقا. 
    
- ضمان استهداف **سياسات التوافق** **وسياسات الوصول المشروط** للمجموعات المطلوبة من المستخدمين. قد يتطلب هذا إنشاء مجموعات معينه من المستخدمين في "Active Directory Azure". 
    
أقرا المزيد:
  
- [أفضل ممارسات الوصول المشروط](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)
    
- [الشروع في التشغيل باستخدام الوصول المشروط](https://docs.microsoft.com/azure/active-directory/active-directory-conditional-access-azure-portal-get-started)
    

