---
title: استكشاف الأخطاء في تلميح الأمان للتحقق من الاحتيال وإصلاحها
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 85faa0086935fb7e7132ee9fdced546bafdb344c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834718"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="d4369-102">استكشاف الأخطاء في تلميح الأمان للتحقق من الاحتيال وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="d4369-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="d4369-103">إذا كنت تحصل على تلميح أمان يقول "فشل المرسل في التحقق من الاحتيال وقد لا يكون الشخص الذي يبدو عليه"، ففشل المرسل في اجتياز أي من فحص مصادقة DKIM أو SPF.</span><span class="sxs-lookup"><span data-stu-id="d4369-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="d4369-104">وأفضل طريقة لحل هذه المشكلة هي أن يفوض المرسل نفسه.</span><span class="sxs-lookup"><span data-stu-id="d4369-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="d4369-105">إذا كان المرسل يرسل بالنيابة عنك، يجب تخويله بإضافة عنوان IP الخاص به إلى سجل SPF الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="d4369-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="d4369-106">راجع استكشاف الأخطاء في تلميح الأمان [الأحمر (المريب)](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) وإصلاحها للتحقق من الكشف عن الاحتيال للحصول على مزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="d4369-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="d4369-107">فيما يلي بعض الارتباطات الأخرى التي يمكن أن تساعدك:</span><span class="sxs-lookup"><span data-stu-id="d4369-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="d4369-108">كيفية استخدام Microsoft إطار نهج المرسل (SPF) لمنع الانتحال</span><span class="sxs-lookup"><span data-stu-id="d4369-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="d4369-109">إعداد SPF للمساعدة في منع التهزاء</span><span class="sxs-lookup"><span data-stu-id="d4369-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-spf-in-office-365-to-help-prevent-spoofing)
