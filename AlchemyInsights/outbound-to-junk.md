---
title: البريد الكتروني الصادر إلى مجلد البريد الكتروني غير الهام
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2697"
ms.assetid: ''
ms.openlocfilehash: 7e6f8d1a161d3eee398230750cc98a46579a56b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47769170"
---
# <a name="outbound-email-to-junk-email-folder"></a><span data-ttu-id="84f3c-102">البريد الكتروني الصادر إلى مجلد البريد الكتروني غير الهام</span><span class="sxs-lookup"><span data-stu-id="84f3c-102">Outbound email to Junk Email folder</span></span>

<span data-ttu-id="84f3c-103">إذا كنت تري الرسائل الصادرة التي تم وضع علامة عليها كبريد غير هام ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="84f3c-103">If you're seeing outbound messages being marked as Junk, do the following steps:</span></span>

- <span data-ttu-id="84f3c-104">إذا لم تكن قد فعلت ذلك ، فعليك [تكوين اعلامات نهج البريد العشوائي الصادرة](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span><span class="sxs-lookup"><span data-stu-id="84f3c-104">If you haven't already, consider [configuring outbound spam policy notifications](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy).</span></span>

- <span data-ttu-id="84f3c-105">استخدم [تتبع الرسائل](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) لمعرفه ما إذا كانت الرسالة الصادرة تتضمن قيمه الحدث غير **المرغوب** فيها باستخدام التفاصيل الاضافيه: **استخدم تجمع التسليم عالي المخاطرة**.</span><span class="sxs-lookup"><span data-stu-id="84f3c-105">Use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc) to see if the outbound message has the event value **Spam** with the additional detail: **Use high risk delivery pool**.</span></span>

  <span data-ttu-id="84f3c-106">بالنسبة إلى هذه الرسائل ، يمكنك التحقق من محتوي الرسالة للاطلاع علي الإجراءات التي تعتبر بريدا عشوائيا.</span><span class="sxs-lookup"><span data-stu-id="84f3c-106">For these messages, check the message content to see what might be considered spam.</span></span> <span data-ttu-id="84f3c-107">علي سبيل المثال ، قد تؤدي التواقيع أحيانا إلى مشاكل في العديد من المستخدمين.</span><span class="sxs-lookup"><span data-stu-id="84f3c-107">For example, signatures can sometimes cause problems for many users.</span></span>

  <span data-ttu-id="84f3c-108">إذا كان لديك العديد من الامثله عن الرسائل الصادرة الشرعية التي تم وضع علامة عليها كبريد غير هام ، فافتح بطاقة دعم واطلب من عامل الدعم إرسال الرسائل كبوسيتيفيس false إلى محللي البريد العشوائي لدينا.</span><span class="sxs-lookup"><span data-stu-id="84f3c-108">If you have multiple examples of legitimate outbound messages that are being marked as Junk, open a support ticket and ask the support agent to submit your messages as false positives to our spam analysts.</span></span> <span data-ttu-id="84f3c-109">كن مستعدا لتوفير الرسائل النموذجية التي تتضمن كل رؤوس الرسائل.</span><span class="sxs-lookup"><span data-stu-id="84f3c-109">Be prepared to provide sample messages that include all message headers.</span></span>
