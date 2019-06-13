---
title: تم رفض الوصول عند عرض سير العمل
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883578"
---
# <a name="access-denied-when-viewing-a-workflow"></a>تم رفض الوصول عند عرض سير العمل

قد يفشل SharePoint 2013 مهام سير العمل التي تحاول إرسال بريد إلكتروني لمجموعة SharePoint مع رسالة خطأ "تم رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint للجميع.
  
 **لحل هذه المشكلة، قم بالخطوات التالية:**
  
 1. السماح للجميع لرؤية أعضاء مجموعة SharePoint.
  
 2. إزالة مجموعة SharePoint من "إلى" أو "نسخة" سطر رسالة البريد الإلكتروني.
  
 3. إضافة المستخدمين بشكل صريح إلى المربع إلى أو نسخة خطية إذا لا يمكن تغيير رؤية العضوية لمجموعة SharePoint.
  
لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير المخول ل/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  