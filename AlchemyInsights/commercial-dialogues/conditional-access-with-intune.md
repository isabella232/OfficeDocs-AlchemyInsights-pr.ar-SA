---
title: استخدام الوصول الشرطي مع Intune
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
- "6700002"
- "7680"
ms.openlocfilehash: 6e86c6b4c9c6adcbeac504acd5a10f2139d04237
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743098"
---
# <a name="using-conditional-access-with-intune"></a><span data-ttu-id="fe535-102">استخدام الوصول الشرطي مع Intune</span><span class="sxs-lookup"><span data-stu-id="fe535-102">Using Conditional Access with Intune</span></span>

<span data-ttu-id="fe535-103">يتطلب استخدام الوصول الشرطي مع Intune 3 خطوات:</span><span class="sxs-lookup"><span data-stu-id="fe535-103">Using Conditional Access with Intune requires 3 steps:</span></span>

- [<span data-ttu-id="fe535-104">قم بإنشاء نهج التوافق لتحديد الإعدادات التي يجب أن يتم التحقق من مطابقتها قبل أن يعتبر الجهاز متوافقا. على سبيل المثال، يجب أن يكون لدى الجهاز دبوس من 6 أرقام على الأقل قبل أن يعتبر متوافقا.</span><span class="sxs-lookup"><span data-stu-id="fe535-104">Create a Compliance Policy to define settings that must be met before the device is considered compliant. For example, a device must have a pin of at least 6 digits before it is considered compliant.</span></span>](https://docs.microsoft.com/mem/intune/protect/create-compliance-policy)
- [<span data-ttu-id="fe535-105">أنشئ نهج الوصول الشرطي الذي يحدد الموارد التي يتم حمايتها، والشروط التي يجب أن يتم توفيرها للوصول إلى تلك الموارد. على سبيل المثال، يجب أن يكون الجهاز متوافقا قبل الوصول إلى البريد الإلكتروني الخاص بالشركة.</span><span class="sxs-lookup"><span data-stu-id="fe535-105">Create a Conditional Access Policy that defines what resources are being protected, and what conditions need to be met to access those resources. For example, a device must be compliant before accessing corporate email.</span></span>](https://docs.microsoft.com/mem/intune/protect/tutorial-protect-email-on-unmanaged-devices#create-conditional-access-policies)
- [<span data-ttu-id="fe535-106">تأكد من أن كل من "سياسات التوافق" و"سياسات الوصول الشرطي" تستهدف مجموعات المستخدمين المطلوبة. قد يتطلب ذلك إنشاء مجموعات معينة من المستخدمين في Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="fe535-106">Ensure both Compliance Policies and Conditional Access Policies are targeted to the desired groups of users. This may require creating specific groups of users in Azure Active Directory.</span></span>](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-conditional-access)

[<span data-ttu-id="fe535-107">قراءة المزيد...</span><span class="sxs-lookup"><span data-stu-id="fe535-107">Read more...</span></span>](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)
