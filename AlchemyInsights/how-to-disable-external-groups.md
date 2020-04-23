---
title: كيفية تعطيل المجموعات الخارجية
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 2159feb4aa3999072de57d76790a2959c7355976
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43720755"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="bdcb3-102">كيفية تعطيل المجموعات الخارجية</span><span class="sxs-lookup"><span data-stu-id="bdcb3-102">How to disable External Groups</span></span>

<span data-ttu-id="bdcb3-103">تطبق الرسائل الخارجية Yammer قواعد نقل Exchange (ETRs)، وهي مجموعة من عناصر التحكم الاستباقية لمنع مشاركة معلومات الشركة.</span><span class="sxs-lookup"><span data-stu-id="bdcb3-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="bdcb3-104">لتقييد المستخدمين من إنشاء مجموعات خارجية، تحتاج إلى تكوين قاعدة نقل Exchange (ETR)، ثم تكوين Yammer لاستخدام قاعدة Exchange Transport لمنع المراسلة الخارجية.</span><span class="sxs-lookup"><span data-stu-id="bdcb3-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="bdcb3-105">بمجرد إنشاء قاعدة في مركز إدارة Exchange Online، اتبع هذه الخطوات لتعيين ETR للتطبيق في Yammer:</span><span class="sxs-lookup"><span data-stu-id="bdcb3-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="bdcb3-106">قم بتسجيل الدخول إلى Yammer كمسؤول تم التحقق منه، وفي **مركز مسؤول Yammer**، انتقل إلى إعدادات أمان المحتوى والأمان \*\* \> C.\*\*</span><span class="sxs-lookup"><span data-stu-id="bdcb3-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="bdcb3-107">ضمن **المراسلة الخارجية،** حدد **فرض قواعد نقل التبادل عبر الإنترنت (ETRs) في Yammer.**</span><span class="sxs-lookup"><span data-stu-id="bdcb3-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="bdcb3-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="bdcb3-108">Choose **Save**.</span></span>

<span data-ttu-id="bdcb3-109">لمزيد من المعلومات، راجع [تعطيل المراسلة الخارجية في شبكة Yammer](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="bdcb3-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  