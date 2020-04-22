---
title: تم رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: c576bf88225582f2577e0b59506a7482cf9f38d5
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687317"
---
# <a name="access-denied-when-viewing-a-workflow"></a>تم رفض الوصول عند عرض سير عمل

يمكن أن تفشل سير عمل SharePoint 2013 التي تحاول إرسال بريد إلكتروني إلى مجموعة SharePoint مع رسالة خطأ "رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint إلى الجميع.
  
 **لحل هذه المشكلة، قم بالخطوات التالية:**
  
 1. السماح للجميع برؤية أعضاء مجموعة SharePoint.
  
 2. قم بإزالة مجموعة SharePoint من سطر To أو CC من البريد الإلكتروني.
  
 3. إضافة المستخدمين بشكل صريح إلى سطر إلى أو نسخة إذا تعذر تغيير رؤية العضوية لمجموعة SharePoint.
  
للاطلاع على مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير مصرح به إلى / _vti_bin/client.svc/sp.utility.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  