---
title: 1554 خطا Winsock 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1554"
- "9000079"
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 4f8007bd8ccb4666260c75fdca15dd0b14eb4e96
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47698849"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="9fda8-102">خطا Winsock 10061</span><span class="sxs-lookup"><span data-stu-id="9fda8-102">Winsock error 10061</span></span>

<span data-ttu-id="9fda8-103">يشير رمز الخطا هذا إلى تعذر علي Microsoft إنشاء ماخذ توصيل TCP (اتصال) مع المضيف الهدف.</span><span class="sxs-lookup"><span data-stu-id="9fda8-103">This error code means that Microsoft couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="9fda8-104">السبب المحتمل هو وجود مشكله في تكوين جدار الحماية.</span><span class="sxs-lookup"><span data-stu-id="9fda8-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="9fda8-105">لإصلاح المشكلة ، تحقق من الإعدادات التالية:</span><span class="sxs-lookup"><span data-stu-id="9fda8-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="9fda8-106">التحقق من تكوين جدار الحماية باستخدام المعلومات الموجودة في [نطاقات عناوين url و Microsoft 365](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="9fda8-106">Verify your firewall configuration with the information in [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="9fda8-107">إذا كان الخطا خاصا ب Exchange Online Protection (EOP) ، فمن المفترض ان تكون قد تم اعلامك مسبقا بتغيير في [عناوين IP ل Exchange Online Protection](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span><span class="sxs-lookup"><span data-stu-id="9fda8-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="9fda8-108">تاكد من ان موفر خدمه الإنترنت (ISP) لا يقوم بحظر المنفذ.</span><span class="sxs-lookup"><span data-stu-id="9fda8-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="9fda8-109">تحقق من إعدادات خادم المضيف الذكي والهدف في الموصلات.</span><span class="sxs-lookup"><span data-stu-id="9fda8-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="9fda8-110">لاحظ ان Microsoft 365 لا يقوم بحظر الاتصالات *الواردة* بهذه الطريقة.</span><span class="sxs-lookup"><span data-stu-id="9fda8-110">Note that Microsoft 365 doesn't block *incoming* connections in this manner.</span></span>
