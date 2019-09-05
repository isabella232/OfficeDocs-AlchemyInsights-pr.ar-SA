---
title: كيفية تعطيل المجموعات الخارجية
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36739480"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="c01c9-102">كيفية تعطيل المجموعات الخارجية</span><span class="sxs-lookup"><span data-stu-id="c01c9-102">How to disable External Groups</span></span>

<span data-ttu-id="c01c9-103">تطبيق المراسلة الخارجية Yammer قواعد نقل Exchange (ETRs) ، مجموعة من عناصر التحكم الاستباقية لمنع مشاركة معلومات الشركة.</span><span class="sxs-lookup"><span data-stu-id="c01c9-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="c01c9-104">لتقييد المستخدمين من إنشاء مجموعات خارجية تحتاج إلى تكوين قاعدة نقل Exchange (ETR) ثم قم بتكوين Yammer لاستخدام قاعدة Exchange Transport لحظر المراسلة الخارجية.</span><span class="sxs-lookup"><span data-stu-id="c01c9-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="c01c9-105">بمجرد إنشاء قاعدة في مركز مسؤول Exchange عبر إنترنت، اتبع الخطوات التالية لتعيين ETR لتطبيق في Yammer:</span><span class="sxs-lookup"><span data-stu-id="c01c9-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="c01c9-106">قم بتسجيل الدخول إلى Yammer كمسؤول تم التحقق منه، وفي **مركز مسؤول Yammer**، انتقل إلى **إعدادات الأمان والمحتوى \> C.**</span><span class="sxs-lookup"><span data-stu-id="c01c9-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="c01c9-107">ضمن **المراسلة الخارجية**، حدد **فرض قواعد النقل Exchange عبر إنترنت (ETRs) في Yammer.**</span><span class="sxs-lookup"><span data-stu-id="c01c9-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="c01c9-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="c01c9-108">Choose **Save**.</span></span>

<span data-ttu-id="c01c9-109">لمزيد من المعلومات، راجع [تعطيل المراسلة الخارجية في شبكة Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="c01c9-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  