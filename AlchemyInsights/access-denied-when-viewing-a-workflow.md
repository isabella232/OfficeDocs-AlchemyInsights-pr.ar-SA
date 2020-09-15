---
title: رفض الوصول عند عرض سير عمل
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688789"
---
# <a name="access-denied-when-viewing-a-workflow"></a>رفض الوصول عند عرض سير عمل

يمكن ان تفشل مهام سير عمل SharePoint 2013 التي تحاول إرسال رسالة بريد الكتروني إلى مجموعه SharePoint مع ظهور رسالة الخطا "رفض الوصول" إذا لم يتم تعيين عضويه مجموعه SharePoint إلى الجميع.
  
 **لحل هذه المشكلة ، قم بتنفيذ الخطوات التالية:**
  
 1. اسمح لجميع برؤية أعضاء مجموعه SharePoint.
  
 2. أزاله مجموعه SharePoint من السطر "إلى" أو "نسخه" في البريد الكتروني.
  
 3. أضف المستخدمين بشكل صريح إلى السطر إلى أو نسخه إذا تعذر تغيير امكانيه رؤية العضوية لمجموعه SharePoint.
  
لعرض المزيد من التفاصيل يرجى الاشاره إلى [HTTP غير مرخص ل/_vti_bin/client.svc/sp.utilities.utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  