---
title: استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c62186fd346efd539b13cef9c80f5e797ebf80811a21db73f0f07fd86c080d55
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939870"
---
# <a name="troubleshoot-access-denied-messages"></a>استكشاف الأخطاء في الرسائل التي تم رفض الوصول إليها وإصلاحها

إذا تلقيت رسالة "تم رفض الوصول" إلى أحد المجلدات المشتركة في SharePoint، فقد يكون مسؤول مجموعة المواقع المشتركة قد قام بتمكين "وضع تأمين إذن الوصول المحدود للمستخدم". إيقاف تشغيل هذا: 
  
1. استعرض بحثا عن الموقع، وانقر فوق أيقونة الإعدادات، ثم انقر فوق **موقع** الإعدادات .
    
2. ضمن **إدارة مجموعة المواقع،** انقر فوق **ميزات مجموعة المواقع.**
    
3. بجانب وضع تأمين إذن الوصول **المحدود للمستخدم،** انقر فوق **إلغاء تنشيط**.
    
يمكن أن تظهر أيضا رسالة رفض الوصول للمجلدات المشتركة إذا كان الموقع موقع نشر. للحصول على معلومات، راجع [رفض الوصول عند الوصول إلى مجلد مشترك](https://answers.microsoft.com/windows/forum/windows_7-files/access-denied-to-share-folder/79fae49d-cddf-4845-8ac8-c141884d85fb).
  
إذا تلقيت رسالة "تم رفض الوصول" من قبل أحد الأشخاص عند محاولة عرض طلبات الوصول، يجب إضافة المستخدم كمسؤول مجموعة مواقع ويب أو كعضو في مجموعة "المالكون" للموقع. لمزيد من المعلومات، راجع [قائمة طلبات الوصول](https://go.microsoft.com/fwlink/?linkid=2004220)التي تم رفض الوصول إليها .
  
إذا تلقيت مستخدم رسالة "رفض الوصول" بعد إزالته من Active Directory في الموقع ثم إضافته مرة أخرى، فشاهد [رفض](https://go.microsoft.com/fwlink/?linkid=2004318)الوصول عند مزامنة حساب مستخدم Microsoft 365 .
  

