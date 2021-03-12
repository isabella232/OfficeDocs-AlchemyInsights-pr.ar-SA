---
title: مثال على نهج المرفق الآمن ل Microsoft Defender ل Office 365
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
ms.openlocfilehash: 077762dd37a2974b4e519c1f242fa753623cb49a
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743093"
---
# <a name="example-microsoft-defender-for-office-365-safe-attachment-policy"></a><span data-ttu-id="b3092-102">مثال على نهج المرفق الآمن ل Microsoft Defender ل Office 365</span><span class="sxs-lookup"><span data-stu-id="b3092-102">Example Microsoft Defender for Office 365 Safe Attachment policy</span></span>

<span data-ttu-id="b3092-103">تمكن هذه الإعدادات  نهج يسمى بلا تأخيرات التي تقوم بتسليم الرسائل على الفور ثم إعادة إرفاق المرفقات بعد فحصها ضوئيا:</span><span class="sxs-lookup"><span data-stu-id="b3092-103">These settings enable a policy called *No delays* that delivers messages immediately and then reattaches attachments after they're scanned:</span></span>

- <span data-ttu-id="b3092-104">**الاسم**: لا توجد تأخيرات</span><span class="sxs-lookup"><span data-stu-id="b3092-104">**Name**: No delays</span></span>
- <span data-ttu-id="b3092-105">**الوصف:** يتم تسليم الرسائل على الفور ثم إعادة إرفاق المرفقات بعد الفحص.</span><span class="sxs-lookup"><span data-stu-id="b3092-105">**Description**: Delivers messages immediately and reattaches attachments after scanning.</span></span>
- <span data-ttu-id="b3092-106">**الاستجابة**: حدد الخيار **تسليم ديناميكي.**</span><span class="sxs-lookup"><span data-stu-id="b3092-106">**Response**: Select the **Dynamic Delivery** option.</span></span> <span data-ttu-id="b3092-107">لمزيد من المعلومات، راجع [التسليم الديناميكي في سياسات المرفقات الآمنة](https://go.microsoft.com/fwlink/?linkid=2092328).</span><span class="sxs-lookup"><span data-stu-id="b3092-107">For more information, see [Dynamic Delivery in Safe Attachments policies](https://go.microsoft.com/fwlink/?linkid=2092328).</span></span>
- <span data-ttu-id="b3092-108">**مقطع إعادة** توجيه المرفقات: حدد الخيار لتمكين إعادة التوجيه **،** ثم أدخل عنوان البريد الإلكتروني لمسؤول Microsoft 365 العام أو مسؤول الأمان أو محلل الأمان الذي سيتحقق من المرفقات الضارة.</span><span class="sxs-lookup"><span data-stu-id="b3092-108">**Redirect attachment** section: Select the option to **Enable redirect**, and then enter the email address of your Microsoft 365 global administrator, security administrator, or security analyst who will investigate malicious attachments.</span></span>
- <span data-ttu-id="b3092-109">**مقطع مطبق** على: **حدد مجال المستلم هو**، ثم حدد مجالك.</span><span class="sxs-lookup"><span data-stu-id="b3092-109">**Applied To** section: Select **The recipient domain is**, and then select your domain.</span></span> <span data-ttu-id="b3092-110">حدد **إضافة**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="b3092-110">Select **add**, and then select **OK**.</span></span> <span data-ttu-id="b3092-111">بمجرد الانتهاء، حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="b3092-111">Once you're finished, select **Save**.</span></span>

<span data-ttu-id="b3092-112">لمعرفة المزيد، راجع [المرفقات الآمنة في Microsoft Defender ل Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span><span class="sxs-lookup"><span data-stu-id="b3092-112">To learn more, see [Safe Attachments in Microsoft Defender for Office 365](https://go.microsoft.com/fwlink/?linkid=2092213).</span></span>
