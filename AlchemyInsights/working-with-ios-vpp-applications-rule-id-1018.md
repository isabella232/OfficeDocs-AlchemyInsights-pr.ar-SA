---
title: العمل باستخدام معرف قاعده تطبيقات iOS فب 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688933"
---
# <a name="working-with-ios-vpp-applications"></a>استخدام تطبيقات iOS فب

أقرا [كيفيه أداره تطبيقات iOS التي تم شراؤها من خلال برنامج لشراء وحده التخزين باستخدام Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) للتعرف علي الميزات والقيود والخطوات المتعلقة باستخدام برنامج الشراء الخاص بوحدات التخزين التي تستخدمها والدعم لها في Microsoft intune.
  
 **المشاكل الشائعة:** "لقد قمت بتعيين تطبيق iOS فب للمستخدمين ، ولكن فشل التثبيت."
  
- قد يحدث هذا في حاله استخدام رمز مميز لفب واحده علي العديد من موفري أداره الاجهزه المحمولة. يمكن استخدام الرموز المميزة لفب من Apple فقط مع موفر واحد. إذا استخدمت رمزا مميزا لفب مع عده موفرين ، فيجب أعاده تحميل الرمز المميز إلى Intune.

- يمكن ان يفشل التثبيت أيضا إذا تجاوز عدد التثبيتات الإجمالي عدد التراخيص. لعرض تقرير استخدام للتراخيص ، انتقل إلى صفحه تراخيص تطبيق **تطبيقات الاجهزه المحمولة في Intune** \> **App licenses** . لمعرفه كيفيه استرداد التراخيص المستخدمة ، راجع [هذه المقالة.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)
