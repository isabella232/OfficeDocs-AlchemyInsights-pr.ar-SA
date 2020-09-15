---
title: استكشاف أخطاء التحقق من الاحتيال وإصلاحها
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: e42b498070bf5d9bfc36110667da8cc0fd431524
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658397"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="ff30a-102">استكشاف أخطاء التحقق من الاحتيال وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="ff30a-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="ff30a-103">إذا كنت تحصل علي تلميح أمان يقول "فشل المرسل في التحقق من البحث عن الاحتيال الخاص بنا وقد لا يكون من يبدو انه" ، فهذا يعني ان المرسل لم يتمكن من تمرير اي من المستخدمين الذين لديهم اي من اليم إلى DKIM SPF.</span><span class="sxs-lookup"><span data-stu-id="ff30a-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="ff30a-104">أفضل طريقه لحل هذه المشكلة هي لتخويل المرسل نفسه.</span><span class="sxs-lookup"><span data-stu-id="ff30a-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="ff30a-105">إذا كان المرسل يرسل بالنيابة عنك ، فيجب عليك تخويله عن طريق أضافه عنوان IP الخاص بالمرسل إلى سجل SPF.</span><span class="sxs-lookup"><span data-stu-id="ff30a-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="ff30a-106">راجع [استكشاف أخطاء تلميح الأمان الأحمر (المشبوه) للتحقق من اكتشاف الاحتيال](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) للحصول علي مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="ff30a-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="ff30a-107">اليك بعض الارتباطات الأخرى التي يمكنها مساعدتك:</span><span class="sxs-lookup"><span data-stu-id="ff30a-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="ff30a-108">كيفيه استخدام Microsoft لاطار عمل نهج المرسل (SPF) لمنع الانتحال</span><span class="sxs-lookup"><span data-stu-id="ff30a-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="ff30a-109">اعداد SPF للمساعدة علي منع الانتحال</span><span class="sxs-lookup"><span data-stu-id="ff30a-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
