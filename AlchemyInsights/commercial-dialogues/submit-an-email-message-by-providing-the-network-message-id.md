---
title: إرسال رسالة بريد إلكتروني من خلال توفير "معرّف رسالة الشبكة"
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: e4a0a3d9b4fede9198c8a235d05945b30a6e0807
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743017"
---
# <a name="submit-an-email-message-by-providing-the-network-message-id"></a><span data-ttu-id="4c395-102">إرسال رسالة بريد إلكتروني من خلال توفير "معرّف رسالة الشبكة"</span><span class="sxs-lookup"><span data-stu-id="4c395-102">Submit an email message by providing the network message ID</span></span>

1. <span data-ttu-id="4c395-103">في قائمة **الإرسال الجديدة،** حدد **البريد الإلكتروني** **ومحدد رسالة الشبكة**.</span><span class="sxs-lookup"><span data-stu-id="4c395-103">In the **New submission** flyout, select **Email** and **Network Message ID**.</span></span>
2. <span data-ttu-id="4c395-104">اتبع هذه الخطوات للعثور على "عرف الرسالة" لرسالة بريد إلكتروني في Outlook:</span><span class="sxs-lookup"><span data-stu-id="4c395-104">Follow these steps to find the message ID for an email message in Outlook:</span></span>
    1. <span data-ttu-id="4c395-105">انقر نقرا مزدوجا فوق رسالة البريد الإلكتروني لفتحها.</span><span class="sxs-lookup"><span data-stu-id="4c395-105">Double-click the email message to open it.</span></span>
    1. <span data-ttu-id="4c395-106">حدد **خصائص**  >  **الملف**.</span><span class="sxs-lookup"><span data-stu-id="4c395-106">Select **File** > **Properties**.</span></span>
    1. <span data-ttu-id="4c395-107">افتح "المفكرة" أو مستند Word فارغ، ثم انسخ المحتوى الذي تم العثور عليه في مربع رؤوس الإنترنت ولصقه في المستند المفتوح ورؤية أفضل. </span><span class="sxs-lookup"><span data-stu-id="4c395-107">Open Notepad or a blank Word document, and then copy and paste the content found in the **Internet headers** box into the open document for better visibility.</span></span>
    1. <span data-ttu-id="4c395-108">حدد موقع **الحقل X-MS-Exchange-Organization-Network-Message-Id.**</span><span class="sxs-lookup"><span data-stu-id="4c395-108">Locate the **X-MS-Exchange-Organization-Network-Message-Id** field.</span></span> <span data-ttu-id="4c395-109">القيمة بعد **:** هي الم ID الذي تحتاج إليه للتقديم.</span><span class="sxs-lookup"><span data-stu-id="4c395-109">The value after the **:** is the ID you need for your submission.</span></span>
3. <span data-ttu-id="4c395-110">ضمن **المستلمون**، إذا تم إرسال البريد الإلكتروني إلى مجلد البريد الإلكتروني غير الهام لجميع مستلمي هذا البريد الإلكتروني، **فاختر تحديد الكل**.</span><span class="sxs-lookup"><span data-stu-id="4c395-110">Under **Recipients**, if the email landed in the junk mail folder for all recipients of this email, choose **Select All**.</span></span> <span data-ttu-id="4c395-111">إذا لم يكن الأمر كذلك، فحدد المستخدم الذي قام ب التقارير عن المشكلة فقط.</span><span class="sxs-lookup"><span data-stu-id="4c395-111">If not, select only the user who reported the issue.</span></span>
4. <span data-ttu-id="4c395-112">ضمن **سبب الإرسال**، إذا قمت بتحديد يجب أن يكون قد تم حظره ، فحدد ما إذا كان يجب حظر الرسالة كرسالة عشوائية أو تصيد احتيالي أو برامج ضارة ، ثم حدد **إرسال**.  </span><span class="sxs-lookup"><span data-stu-id="4c395-112">Under **Reason for submission**, if you select **Should have been blocked**, specify whether the message should have been blocked as **Spam**, **Phishing**, or **Malware**, and then select **Submit**.</span></span>

<span data-ttu-id="4c395-113">لمعرفة المزيد، راجع كيفية إرسال البريد العشوائي والتصيد الاحتيالي عناوين URL والملفات المشتبه بها إلى [Microsoft للفحص.](https://go.microsoft.com/fwlink/?linkid=2101479)</span><span class="sxs-lookup"><span data-stu-id="4c395-113">To learn more, see [How to submit suspected spam, phish, URLs, and files to Microsoft for scanning](https://go.microsoft.com/fwlink/?linkid=2101479).</span></span>
