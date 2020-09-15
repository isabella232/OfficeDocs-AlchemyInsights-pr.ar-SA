---
title: 2589 تعليمات حول منع المرفقات مرفق winmail.dat في رسائل البريد الكتروني من المؤسسة
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2589
ms.assetid: ''
ms.openlocfilehash: f67c4146af419a590651c8e0673fd59fabd7eae7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47693722"
---
# <a name="help-prevent-winmaildat-attachments-in-email-messages-from-your-organization"></a><span data-ttu-id="f6467-102">المساعدة علي منع مرفقات مرفق winmail.dat في رسائل البريد الكتروني من المؤسسة</span><span class="sxs-lookup"><span data-stu-id="f6467-102">Help prevent Winmail.dat attachments in email messages from your organization</span></span>

<span data-ttu-id="f6467-103">بصفتك المسؤول ، جرب الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f6467-103">As an admin, try these steps:</span></span>

1. <span data-ttu-id="f6467-104">افتح [مركز أداره Exchange](https://outlook.office365.com/ecp/).</span><span class="sxs-lookup"><span data-stu-id="f6467-104">Open the [Exchange admin center](https://outlook.office365.com/ecp/).</span></span>

2. <span data-ttu-id="f6467-105">انتقل إلى **Mail flow**  >  **المجالات البعيدة**لتدفق البريد.</span><span class="sxs-lookup"><span data-stu-id="f6467-105">Go to **Mail flow** > **Remote domains**.</span></span>

3. <span data-ttu-id="f6467-106">حدد المجال البعيد الافتراضي المسمي **افتراضي**، ثم انقر فوق **تحرير**.</span><span class="sxs-lookup"><span data-stu-id="f6467-106">Select the default remote domain named **Default**, and then click **Edit**.</span></span>

4. <span data-ttu-id="f6467-107">في المقطع **استخدام تنسيق النص المنسق** ، حدد **أبدا**.</span><span class="sxs-lookup"><span data-stu-id="f6467-107">In the **Use Rich-text format** section, select **Never**.</span></span>

<span data-ttu-id="f6467-108">لمزيد من المعلومات ، راجع [تحديد تنسيق الرسالة للمجالات البعيدة](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span><span class="sxs-lookup"><span data-stu-id="f6467-108">For more information, see [Specify the message format for remote domains](https://docs.microsoft.com/Exchange/mail-flow-best-practices/remote-domains/remote-domains#specifying-message-format).</span></span>
