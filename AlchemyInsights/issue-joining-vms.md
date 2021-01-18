---
title: الانضمام إلى VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884804"
---
# <a name="issue-joining-vms"></a>الانضمام إلى VMs

لحل المشاكل التي تحدث اثناء محاولة الانضمام إلى VMs ، نفذ الخطوات التالية:

1. حاول تسجيل الدخول باستخدام تنسيق **UPN** (علي سبيل المثال ، ' joeuser@contoso.com ') بدلا من تنسيق **ساماككونتنامي** (' contoso\joeuser ').
2. تاكد من انك قمت بتمكين مزامنة كلمه المرور بالتوافق مع الخطوات المذكورة في دليل *بدء* الاستخدام.
3. تاكد من ان حساب المستخدم المتاثر ليس حسابا خارجيا في مستاجر Azure AD. لا يمكن للمستخدمين الخارجيين تسجيل الدخول إلى المجال المدار بما ان خدمات مجال Azure AD لا تملك بيانات اعتماد لحسابات المستخدمين هذه.
4. إذا كان حساب المستخدم المتاثر هو حساب مستخدم خاص بالسحابة ، فتاكد من قيام المستخدمين بتغيير كلمه المرور الخاصة بهم بعد تمكين خدمات مجالات Azure AD. تؤدي هذه الخطوة إلى إنشاء تجزئات بيانات الاعتماد المطلوبة لخدمات مجال Azure AD.
5. إذا تمت مزامنة حسابات المستخدمين المتاثرين من دليل محلي ، فتاكد من تكوين الإصدار الموصي به من Azure AD Connect لاجراء مزامنة كامله.
6. إذا استمرت المشاكل بعد تاكيد الخطوة 4 ، فقم بتنفيذ الأوامر التالية من جهاز المزامنة:
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.