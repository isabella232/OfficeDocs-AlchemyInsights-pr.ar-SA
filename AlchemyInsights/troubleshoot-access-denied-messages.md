---
title: استكشاف رسائل رفض الوصول وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 6c8ad84123fb58b73b9c378592ce970997893ea2
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704881"
---
# <a name="troubleshoot-access-denied-messages"></a>استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها

إذا تلقيت رسالة "رفض الوصول" إلى أحد المجلدات المشتركة في SharePoint، فقد يكون مسؤول مجموعة المواقع المشتركة قد قام بتمكين "وضع تأمين إذن المستخدم للوصول المحدود". إيقاف تشغيل هذا: 
  
1. استعرض بحثا عن الموقع، وانقر فوق الأيقونة "إعدادات"، ثم انقر فوق **"إعدادات الموقع".**
    
2. ضمن **إدارة مجموعة المواقع،** انقر فوق **ميزات مجموعة المواقع.**
    
3. بجانب وضع تأمين إذن المستخدم للوصول **المحدود،** انقر **فوق "إلغاء تنشيط".**
    
يمكن أن تظهر رسالة "رفض الوصول" أيضا للمجلدات المشتركة إذا كان الموقع موقع نشر. للحصول على معلومات، راجع ["رفض الوصول" عند الوصول إلى مجلد مشترك.](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb)
  
إذا تلقيت رسالة "رفض الوصول" لأحد الأشخاص عند محاولة عرض طلبات الوصول، يجب إضافة المستخدم كمسؤول مجموعة مواقع ويب أو كعضو في مجموعة "المالكون" للموقع. لمزيد من المعلومات، راجع [القائمة "رفض الوصول إلى طلبات الوصول".](https://go.microsoft.com/fwlink/?linkid=2004220)
  
إذا ظهر للمستخدم رسالة "رفض الوصول" بعد إزالته من Active Directory في الموقع ثم إضافته مرة أخرى، فشاهد "رفض الوصول" عند مزامنة حساب مستخدم مع [Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2004318)
  

