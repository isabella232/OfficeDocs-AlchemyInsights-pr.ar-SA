---
title: كيفية تعطيل "المجموعات الخارجية"
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
ms.openlocfilehash: 95e60599b5298090db23bf887cb860350280964f
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35384812"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="d7e4c-102">كيفية تعطيل "المجموعات الخارجية"</span><span class="sxs-lookup"><span data-stu-id="d7e4c-102">How to disable External Groups</span></span>

<span data-ttu-id="d7e4c-103">Yammer الرسائل الخارجية تطبق قواعد النقل Exchange (ETRs)، مجموعة من عناصر التحكم استباقية لمنع الشركة من المشاركة.</span><span class="sxs-lookup"><span data-stu-id="d7e4c-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="d7e4c-104">لمنع المستخدمين من إنشاء مجموعات خارجية، تحتاج إلى تكوين قاعدة نقل Exchange (العتر)، ثم قم بتكوين Yammer لاستخدام قاعدة النقل Exchange لحظر الرسائل الخارجية.</span><span class="sxs-lookup"><span data-stu-id="d7e4c-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="d7e4c-105">حالما تقوم بإنشاء قاعدة في مركز مسؤول Exchange عبر الإنترنت، اتبع هذه الخطوات لتعيين عطر لتطبيق في Yammer:</span><span class="sxs-lookup"><span data-stu-id="d7e4c-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="d7e4c-106">تسجيل الدخول إلى Yammer كمشرف تم التحقق منها، وفي **Yammer مركز الإدارة**، انتقل إلى ج **المحتوى والأمن \> "إعدادات الأمان"-**</span><span class="sxs-lookup"><span data-stu-id="d7e4c-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="d7e4c-107">ضمن **الرسائل الخارجية**، حدد **فرض "القواعد" الخاصة بك Exchange عبر إنترنت تبادل النقل (ETRs) في Yammer-**</span><span class="sxs-lookup"><span data-stu-id="d7e4c-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="d7e4c-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="d7e4c-108">Choose **Save**.</span></span>

<span data-ttu-id="d7e4c-109">لمزيد من المعلومات، راجع [التحكم بالمراسلة في شبكة Yammer قواعد "تبادل النقل" الخارجي](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="d7e4c-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  