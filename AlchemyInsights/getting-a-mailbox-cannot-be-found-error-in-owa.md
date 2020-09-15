---
title: 126 تعذر العثور علي علبه بريد في OWA ؟
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 9a8897767ebfebac5807116251634c615ef6767d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47706737"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="9e2f1-102">لم يتم العثور علي خطا في الوصول إلى علبه بريد في Outlook علي الويب ؟</span><span class="sxs-lookup"><span data-stu-id="9e2f1-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="9e2f1-103">إذا كنت تستخدم Outlook علي ويب وظهرت رسالة **الخطا تعذر العثور علي علبه بريد** ، فهذا يعني ان الحساب الذي استخدمته للاتصال ب Outlook علي الويب لا يتضمن ترخيص Exchange Online ، التالي لا يتم اقران علبه البريد بالحساب.</span><span class="sxs-lookup"><span data-stu-id="9e2f1-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="9e2f1-104">يمكن للمسؤول تعيين ترخيص لحسابك من خلال اتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9e2f1-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="9e2f1-105">افتح [مركز أداره Microsoft 365](https://portal.office.com/adminportal/home#/homepage) وانتقل إلى **المستخدمون النشطون** ضمن القسم **المستخدمون** ، وحدد المستخدم الذي يري الخطا.</span><span class="sxs-lookup"><span data-stu-id="9e2f1-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="9e2f1-106">في صفحه المستخدم التي تفتح ، انتقل إلى القسم **التراخيص والتطبيقات** ، وحدد قيمه **الموقع** المناسب ، وقم بتعيين ترخيص يحتوي علي Exchange Online (وسع الترخيص للاطلاع علي التفاصيل الخاصة به).</span><span class="sxs-lookup"><span data-stu-id="9e2f1-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="9e2f1-107">عند الانتهاء ، انقر فوق **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="9e2f1-107">When you're finished, click **Save changes**.</span></span>
