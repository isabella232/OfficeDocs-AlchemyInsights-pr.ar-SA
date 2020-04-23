---
title: 1554 Winsock خطأ 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: e8f62d97efc937518ef766b45e1747e83b7f99c3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766156"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="ff264-102">Winsock خطأ 10061</span><span class="sxs-lookup"><span data-stu-id="ff264-102">Winsock error 10061</span></span>

<span data-ttu-id="ff264-103">رمز الخطأ هذا يعني أن Microsoft لم تتمكن من إنشاء مأخذ توصيل TCP (اتصال) مع المضيف الهدف.</span><span class="sxs-lookup"><span data-stu-id="ff264-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="ff264-104">السبب الأكثر احتمالاً لهذا الخطأ هو مشكلة في تكوين جدار الحماية الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="ff264-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="ff264-105">لإصلاح المشكلة، تحقق من هذه الإعدادات:</span><span class="sxs-lookup"><span data-stu-id="ff264-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="ff264-106">التحقق من تكوين جدار الحماية الخاص بك مع المعلومات الموجودة في [عناوين URL Microsoft 365 ونطاقات عناوين IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="ff264-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="ff264-107">إذا كان الخطأ خاصًا بـ Exchange Online Protection (EOP)، فيجب أن يكون قد تم إعلامك مسبقًا بتغيير [عناوين IP الخاصة بحماية Exchange عبر الإنترنت](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="ff264-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="ff264-108">تحقق من أن موفر خدمة الإنترنت (ISP) لا يقوم بحظر المنفذ.</span><span class="sxs-lookup"><span data-stu-id="ff264-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="ff264-109">تحقق من إعدادات المضيف والخادم المستهدف الذكية في الموصلات.</span><span class="sxs-lookup"><span data-stu-id="ff264-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="ff264-110">لاحظ أن Microsoft 365 لا يمنع الاتصالات *الواردة* بهذه الطريقة.</span><span class="sxs-lookup"><span data-stu-id="ff264-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
