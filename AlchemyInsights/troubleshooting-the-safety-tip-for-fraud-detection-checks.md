---
title: التحقق من استكشاف الأخطاء وإصلاحها في رأس الأمان للكشف عن حالات الغش
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 24842e8cc5c6e47fb0eb637e6a3211637ede1ed8
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/15/2019
ms.locfileid: "28273773"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="167a8-102">التحقق من استكشاف الأخطاء وإصلاحها في رأس الأمان للكشف عن حالات الغش</span><span class="sxs-lookup"><span data-stu-id="167a8-102">Troubleshooting the safety tip for fraud detection checks</span></span>

<span data-ttu-id="167a8-p101">في حالة الحصول على تلميح سلامة يقول "المرسل فشل اختبارات الكشف عن الاحتيال الخاصة بنا وقد لا يكون الذين يبدو أنها"، ثم المرسل فشلت عمليات فحص مصادقة DKIM أو منتدى جنوب المحيط الهادئ. أفضل طريقة لحل هذه المشكلة للمرسل أن تأذن لأنفسهم. إذا تم إرسال المرسل بالنيابة عنك، تحتاج تأذن لهم بإضافة عنوان IP الخاص بالمرسل إلى سجلك منتدى جنوب المحيط الهادئ.</span><span class="sxs-lookup"><span data-stu-id="167a8-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="167a8-106">لمزيد من المعلومات، راجع [التحقق من استكشاف الأخطاء وإصلاحها تلميح الأحمر السلامة (المشبوهة) للكشف عن حالات الغش](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="167a8-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="167a8-107">فيما يلي بعض الارتباطات الأخرى التي يمكن أن تساعد:</span><span class="sxs-lookup"><span data-stu-id="167a8-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="167a8-108">كيفية استخدام Office 365 إطار سياسة المرسل (منتدى جنوب المحيط الهادئ) لمنع الانتحال</span><span class="sxs-lookup"><span data-stu-id="167a8-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="167a8-109">إعداد منتدى جنوب المحيط الهادئ في Office 365 لمنع الانتحال</span><span class="sxs-lookup"><span data-stu-id="167a8-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/en-us/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    

