---
title: IP 1264 حظر إرسال بريد إلكتروني عشوائي كبيرة جداً (550 5.7.51)
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1264
ms.assetid: f7af4211-9dbe-415c-b0e3-fc20d43c3868
ms.openlocfilehash: d2d92a15a1863f0c4625fd363096fbfd0582a467
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2019
ms.locfileid: "32409929"
---
# <a name="access-denied-banned-sender"></a><span data-ttu-id="611ae-102">تم رفض الوصول، حظر المرسل</span><span class="sxs-lookup"><span data-stu-id="611ae-102">Access denied, banned sender</span></span>

 <span data-ttu-id="611ae-103">**خطأ**: خطأ SMTP من ملقم بعيد من أجل RCPT للأمر، استضافة: *xxxx*-السبب com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*): 550 5.7.511 الوصول مرفوض، المحظورة المرسل [*xx.xxx.x.xxx*].</span><span class="sxs-lookup"><span data-stu-id="611ae-103">**Error**: SMTP error from remote server for RCPT TO command, host: *xxxx*-com.mail.protection.outlook.com (*xxx.xxx.xxx.xxx*) reason: 550 5.7.511 Access denied, banned sender [*xx.xxx.x.xxx*].</span></span> 

<span data-ttu-id="611ae-104">في حالة ظهور هذا الخطأ عند إرسال بريد إلكتروني إلى مستلم Office 365، إزالة حساب المتأثرة من قائمة المرسلين المحظورين في [https://sender.office.com](https://sender.office.com).</span><span class="sxs-lookup"><span data-stu-id="611ae-104">If you receive this error when sending email to an Office 365 recipient, remove the affected account from the blocked senders list at [https://sender.office.com](https://sender.office.com).</span></span>
