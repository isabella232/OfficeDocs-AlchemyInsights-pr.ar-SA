---
title: خطأ Winsock 1554 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903083"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="46113-102">خطأ Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="46113-102">Winsock error 10061</span></span>

<span data-ttu-id="46113-p101">رمز الخطأ هذا يعني أن Office 365 تعذر إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف. السبب المحتمل لهذا الخطأ مشكلة في تكوين جدار الحماية الخاص بك. لحل هذه المشكلة، تحقق من هذه الإعدادات:</span><span class="sxs-lookup"><span data-stu-id="46113-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="46113-106">تحقق من تكوين جدار الحماية الخاص بك باستخدام المعلومات الموجودة في [Office 365 URLs ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="46113-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="46113-107">إذا كان الخطأ خاص إلى Exchange عبر إنترنت الحماية (البرنامج)، قد يجب أن تم مسبقاً إعلامك لتغيير [عناوين IP في حماية Exchange عبر إنترنت](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="46113-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="46113-108">تأكد من أن موفر خدمة إنترنت (ISP) لا يقوم بحظر المنفذ.</span><span class="sxs-lookup"><span data-stu-id="46113-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="46113-109">تحقق من إعدادات الخادم المضيف والهدف الذكية في الموصلات.</span><span class="sxs-lookup"><span data-stu-id="46113-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="46113-110">لاحظ أن Office 365 لا منع الاتصالات *الواردة* على هذا النحو.</span><span class="sxs-lookup"><span data-stu-id="46113-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

