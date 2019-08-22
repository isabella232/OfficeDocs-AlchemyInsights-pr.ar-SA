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
ms.openlocfilehash: 53bd9285e49e220f880eea21923f261302003127
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495810"
---
# <a name="access-denied-when-viewing-a-workflow"></a>تم رفض الوصول عند عرض سير العمل

قد يفشل SharePoint 2013 مهام سير العمل التي تحاول إرسال بريد إلكتروني لمجموعة SharePoint مع رسالة خطأ "تم رفض الوصول" إذا لم يتم تعيين عضوية مجموعة SharePoint للجميع.
  
 **لحل هذه المشكلة، قم بالخطوات التالية:**
  
 1. السماح للجميع لرؤية أعضاء مجموعة SharePoint.
  
 2. إزالة مجموعة SharePoint من "إلى" أو "نسخة" سطر رسالة البريد الإلكتروني.
  
 3. إضافة المستخدمين بشكل صريح إلى المربع إلى أو نسخة خطية إذا لا يمكن تغيير رؤية العضوية لمجموعة SharePoint.
  
لعرض مزيد من التفاصيل يرجى الرجوع إلى [HTTP غير المخول ل/_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  