---
title: كيفيه تعطيل المجموعات الخارجية
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704115"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="6765e-102">كيفيه تعطيل المجموعات الخارجية</span><span class="sxs-lookup"><span data-stu-id="6765e-102">How to disable External Groups</span></span>

<span data-ttu-id="6765e-103">تطبق المراسلة الخارجية في Yammer قواعد نقل Exchange (Etr) ، وهي مجموعه من عناصر التحكم الاستباقية لمنع مشاركه معلومات الشركة.</span><span class="sxs-lookup"><span data-stu-id="6765e-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="6765e-104">لمنع المستخدمين من إنشاء مجموعات خارجيه ، يجب تكوين قاعده نقل Exchange (اتر) ، ثم قم بتكوين Yammer لاستخدام قاعده نقل Exchange لحظر المراسلة الخارجية.</span><span class="sxs-lookup"><span data-stu-id="6765e-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="6765e-105">بعد إنشاء قاعده في مركز أداره Exchange Online ، اتبع الخطوات التالية لتعيين اتر لتطبيقه في Yammer:</span><span class="sxs-lookup"><span data-stu-id="6765e-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="6765e-106">سجل الدخول إلى Yammer كمسؤول تم التحقق منه ، وفي **مركز أداره Yammer**، انتقل إلى \*\* \> إعدادات الأمان ومحتوي C.\*\*</span><span class="sxs-lookup"><span data-stu-id="6765e-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="6765e-107">ضمن **المراسلة الخارجية**، حدد **فرض قواعد نقل Exchange Online (Etr) في Yammer.**</span><span class="sxs-lookup"><span data-stu-id="6765e-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="6765e-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="6765e-108">Choose **Save**.</span></span>

<span data-ttu-id="6765e-109">لمزيد من المعلومات ، راجع [تعطيل المراسلة الخارجية في شبكه Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="6765e-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  