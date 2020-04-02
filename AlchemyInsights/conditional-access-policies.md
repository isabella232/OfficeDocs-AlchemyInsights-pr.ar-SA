---
title: نهج الوصول المشروط
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100380"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="4511f-102">نهج الوصول المشروط</span><span class="sxs-lookup"><span data-stu-id="4511f-102">Conditional Access policies</span></span>

<span data-ttu-id="4511f-103">الوصول المشروط عبارة عن إمكانية Azure AD التي تمكنك من فرض عناصر تحكم في الوصول إلى التطبيقات الموجودة في بيئتك، كل ذلك بالاستناد إلى شروط معينة وتتم إدارتها من موقع مركزي.</span><span class="sxs-lookup"><span data-stu-id="4511f-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="4511f-104">تعرّف على المزيد حول [الوصول المشروط لـ Azure AD](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="4511f-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="4511f-105">**ملاحظة**: إذا تم إنشاء المستأجر بعد يوم 21 أكتوبر 2019 وتمت مطالبتك بشكل غير متوقع بالمصادقة متعددة العوامل، فمن المحتمل أن تكون قد مكنت، [إعدادات الأمان الافتراضية](http://aka.ms/securitydefaults) في المستأجر.</span><span class="sxs-lookup"><span data-stu-id="4511f-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="4511f-106">**لإدارة إعدادات الأمان الافتراضية**</span><span class="sxs-lookup"><span data-stu-id="4511f-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="4511f-107">سجّل الدخول إلى [مركز الإدارة](https://go.microsoft.com/fwlink/p/?linkid=834822) باستخدام بيانات اعتماد المسؤول العمومي.</span><span class="sxs-lookup"><span data-stu-id="4511f-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="4511f-108">انتقل إلى [خصائص Azure Active Directory](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="4511f-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="4511f-109">في أسفل الصفحة، انقر فوق **إدارة الإعدادات الافتراضية للأمان**.</span><span class="sxs-lookup"><span data-stu-id="4511f-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="4511f-110">انقر فوق **نعم** لتمكين إعدادات الأمان الافتراضية أو**لا** لتعطيل إعدادات الأمان الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="4511f-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
