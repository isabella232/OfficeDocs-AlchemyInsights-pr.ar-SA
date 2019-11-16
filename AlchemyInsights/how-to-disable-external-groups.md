---
title: كيفيه تعطيل المجموعات الخارجية
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
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/15/2019
ms.locfileid: "36739480"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="053e7-102">كيفيه تعطيل المجموعات الخارجية</span><span class="sxs-lookup"><span data-stu-id="053e7-102">How to disable External Groups</span></span>

<span data-ttu-id="053e7-103">تطبيق المراسلة الخارجية Yammer قواعد النقل Exchange (ETRs) ، مجموعه من عناصر التحكم الاستباقية لمنع مشاركه معلومات الشركة.</span><span class="sxs-lookup"><span data-stu-id="053e7-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="053e7-104">لتقييد المستخدمين من إنشاء مجموعات خارجيه تحتاج إلى تكوين قاعده نقل Exchange (ETR) ثم قم بتكوين Yammer لاستخدام قاعده نقل Exchange لحظر المراسلة الخارجية.</span><span class="sxs-lookup"><span data-stu-id="053e7-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="053e7-105">بمجرد إنشاء قاعده في مركز مسؤول Exchange عبر الإنترنت ، اتبع الخطوات التالية لتعيين ETR لتطبيق في Yammer:</span><span class="sxs-lookup"><span data-stu-id="053e7-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="053e7-106">قم بتسجيل الدخول إلى Yammer كمسؤول تم التحقق منه ، وفي **مركز أداره yammer**، انتقل إلى **المحتوي C وإعدادات أمان الأمان \> .**</span><span class="sxs-lookup"><span data-stu-id="053e7-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="053e7-107">ضمن " **المراسلة الخارجية**" ، حدد **فرض Exchange عبر الإنترنت تبادل قواعد النقل (etrs) في Yammer.**</span><span class="sxs-lookup"><span data-stu-id="053e7-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="053e7-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="053e7-108">Choose **Save**.</span></span>

<span data-ttu-id="053e7-109">لمزيد من المعلومات ، راجع [تعطيل المراسلة الخارجية في شبكه Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="053e7-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  