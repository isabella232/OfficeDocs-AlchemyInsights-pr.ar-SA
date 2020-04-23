---
title: استكشاف أخطاء معلومات الأمان للتحقق من اكتشاف الاحتيال
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.custom:
- "275"
- "3100004"
ms.openlocfilehash: 61159391f7a9876750cd7fefc40c54054fb9bec9
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759499"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="42ddc-102">استكشاف أخطاء معلومات الأمان للتحقق من اكتشاف الاحتيال</span><span class="sxs-lookup"><span data-stu-id="42ddc-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="42ddc-103">إذا كنت تحصل على معلومات أمان تقول "فشل المرسل في التحقق من اكتشاف الاحتيال وقد لا يكون ما يبدو أنه عليه"، فقد فشل المرسل في اجتياز عمليات التحقق من مصادقة DKIM أو SPF.</span><span class="sxs-lookup"><span data-stu-id="42ddc-103">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks.</span></span> <span data-ttu-id="42ddc-104">أفضل طريقة لحل هذا هو للمرسل لتخويل أنفسهم.</span><span class="sxs-lookup"><span data-stu-id="42ddc-104">The best method to resolve this is for the sender to authorize themselves.</span></span> <span data-ttu-id="42ddc-105">إذا كان المرسل يرسل نيابة عنك، فستحتاج إلى تخويلها بإضافة عنوان IP الخاص بالمرسل إلى سجل SPF الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="42ddc-105">If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="42ddc-106">راجع [استكشاف الأخطاء وإصلاحها في معلومات الأمان الحمراء (المشبوهة) للتحقق من اكتشاف الاحتيال](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) لمزيد من المعلومات.</span><span class="sxs-lookup"><span data-stu-id="42ddc-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span>
  
<span data-ttu-id="42ddc-107">فيما يلي بعض الروابط الأخرى التي يمكن أن تساعد:</span><span class="sxs-lookup"><span data-stu-id="42ddc-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="42ddc-108">كيف تستخدم Microsoft إطار نهج المرسل (SPF) لمنع الانتحال</span><span class="sxs-lookup"><span data-stu-id="42ddc-108">How Microsoft uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)

- [<span data-ttu-id="42ddc-109">إعداد SPF للمساعدة في منع الانتحال</span><span class="sxs-lookup"><span data-stu-id="42ddc-109">Set up SPF to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
