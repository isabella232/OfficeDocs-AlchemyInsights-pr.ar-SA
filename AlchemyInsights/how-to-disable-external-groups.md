---
title: كيفية تعطيل "المجموعات الخارجية"
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4807dbfbabcea1f13785bd39bb48e4bbaa8d0f0f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29456286"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="57b8d-102">كيفية تعطيل "المجموعات الخارجية"</span><span class="sxs-lookup"><span data-stu-id="57b8d-102">How to disable External Groups</span></span>

<span data-ttu-id="57b8d-p101">Yammer الرسائل الخارجية تطبق قواعد النقل Exchange (ETRs)، مجموعة من عناصر التحكم استباقية لمنع الشركة من المشاركة. لمنع المستخدمين من إنشاء مجموعات خارجية، تحتاج إلى تكوين قاعدة نقل Exchange (العتر)، ثم قم بتكوين Yammer لاستخدام قاعدة النقل Exchange لحظر الرسائل الخارجية.</span><span class="sxs-lookup"><span data-stu-id="57b8d-p101">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared. In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="57b8d-105">حالما تقوم بإنشاء قاعدة في مركز مسؤول Exchange عبر الإنترنت، اتبع هذه الخطوات لتعيين عطر لتطبيق في Yammer:</span><span class="sxs-lookup"><span data-stu-id="57b8d-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="57b8d-106">تسجيل الدخول إلى Yammer كمشرف تم التحقق منها، وفي **Yammer مركز الإدارة**، انتقل إلى ج **فقه على المحتوى والأمن \> "إعدادات الأمان"-**</span><span class="sxs-lookup"><span data-stu-id="57b8d-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="57b8d-107">ضمن **الرسائل الخارجية**، حدد **فرض "القواعد" الخاصة بك Exchange عبر إنترنت تبادل النقل (ETRs) في Yammer-**</span><span class="sxs-lookup"><span data-stu-id="57b8d-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="57b8d-108">اختر **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="57b8d-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="57b8d-109">لمزيد من المعلومات، راجع [التحكم بالمراسلة في شبكة Yammer قواعد "تبادل النقل" الخارجي](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span><span class="sxs-lookup"><span data-stu-id="57b8d-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/en-us/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

