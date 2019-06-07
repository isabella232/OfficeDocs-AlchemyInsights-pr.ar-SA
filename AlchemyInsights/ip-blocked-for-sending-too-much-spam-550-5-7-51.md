---
title: IP 1264 حظر إرسال بريد إلكتروني عشوائي كبيرة جداً (550 5.7.51)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1264
ms.assetid: f7af4211-9dbe-415c-b0e3-fc20d43c3868
ms.openlocfilehash: 64a829ed6e5d0d2a15e4eb4dfb5f70c1bd652ed6
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34751654"
---
# <a name="access-denied-banned-sender"></a><span data-ttu-id="98ef2-102">تم رفض الوصول، حظر المرسل</span><span class="sxs-lookup"><span data-stu-id="98ef2-102">Access denied, banned sender</span></span>

 <span data-ttu-id="98ef2-103">**خطأ**: خطأ SMTP من ملقم بعيد من أجل RCPT للأمر، استضافة: *xxxx*-السبب com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*): 550 5.7.511 الوصول مرفوض، المحظورة المرسل [*xx.xxx.x.xxx*].</span><span class="sxs-lookup"><span data-stu-id="98ef2-103">**Error**: SMTP error from remote server for RCPT TO command, host: *xxxx*-com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*) reason: 550 5.7.511 Access denied, banned sender [*xx.xxx.x.xxx*].</span></span> 

<span data-ttu-id="98ef2-104">في حالة ظهور هذا الخطأ عند إرسال بريد إلكتروني إلى مستلم Office 365، إزالة حساب المتأثرة من قائمة المرسلين المحظورين في [https://sender.office.com](https://sender.office.com).</span><span class="sxs-lookup"><span data-stu-id="98ef2-104">If you receive this error when sending email to an Office 365 recipient, remove the affected account from the blocked senders list at [https://sender.office.com](https://sender.office.com).</span></span>
