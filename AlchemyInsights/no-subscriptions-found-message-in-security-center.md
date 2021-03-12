---
title: لم يتم العثور على أي رسالة اشتراكات في مركز الأمان
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "50713266"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a>لم يتم العثور على أي رسالة اشتراكات في مركز الأمان

إذا حصلت على رسالة "لم يتم العثور على اشتراكات" أثناء الوصول إلى مركز أمان Microsoft Defender، فهذا يعني أن Azure Active Directory (AAD) المستخدم لتسجيل دخول المستخدم إلى المدخل ليس لديه ترخيص MICROSOFT Defender ATP.  

إن تراخيص Windows E5 و Office E5 هي تراخيص منفصلة.

افتح حالة دعم إذا تم شراء الترخيص ولكن لم يتم توفيره لمثيل AAD هذا. إما أن يكون لديك: <br/>
-   مشكلة محتملة في توفير التراخيص.<br/>
-   لقد قمت عن غير قصد بتوفير الترخيص ل Microsoft AAD مختلف عن ذلك المستخدم للمصادقة في الخدمة.