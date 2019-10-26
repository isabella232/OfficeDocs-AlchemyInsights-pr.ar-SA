---
title: تم رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747735"
---
# <a name="access-denied-when-viewing-a-workflow"></a>تم رفض الوصول عند عرض سير عمل

يمكن ان تفشل مهام سير العمل 2013 SharePoint التي تحاول إرسال بريد الكتروني إلى مجموعه SharePoint مع رسالة خطا "تم رفض الوصول" إذا لم يتم تعيين عضويه مجموعه SharePoint إلى Everyone.
  
 **لحل هذه المشكلة ، قم بالخطوات التالية:**
  
 1. السماح للجميع بمشاهده أعضاء مجموعه SharePoint.
  
 2. أزاله مجموعه SharePoint من سطر إلى أو نسخه من البريد الكتروني.
  
 3. قم باضافه المستخدمين بشكل صريح إلى السطر "إلى" أو "نسخه" إذا تعذر تغيير رؤية العضوية لمجموعه SharePoint.
  
لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير مصرح به إلى/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  