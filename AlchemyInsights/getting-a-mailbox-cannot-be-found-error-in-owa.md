---
title: 126 هل يتعذر العثور على خطأ في الحصول على علبة بريد في OWA؟
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
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426649"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="95f23-102">هل لم يتم العثور على رسالة خطأ في علبة البريد في Outlook على الويب؟</span><span class="sxs-lookup"><span data-stu-id="95f23-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="95f23-103">إذا كنت تستخدم Outlook على الويب وعثرت على علبة بريد لخطأ، فإن الحساب الذي استخدمته للاتصال ب Outlook على الويب ليس لديه ترخيص Exchange Online، وبالتالي لا توجد علبة بريد مقترنة بهذا الحساب. </span><span class="sxs-lookup"><span data-stu-id="95f23-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="95f23-104">يمكن للمسؤول تعيين ترخيص لحسابك باتباع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="95f23-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="95f23-105">افتح  [مركز إدارة Microsoft 365](https://portal.office.com/adminportal/home#/homepage) واذهب  إلى المستخدمون النشطون ضمن القسم المستخدمون، وحدد المستخدم الذي يرى الخطأ.</span><span class="sxs-lookup"><span data-stu-id="95f23-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="95f23-106">في صفحة المستخدم التي تفتح،  انتقل إلى المقطع التراخيص  والتطبيقات، وحدد قيمة الموقع المناسبة، ثم عين ترخيصا يحتوي على Exchange Online (قم بتوسيع الترخيص لرؤية تفاصيله).</span><span class="sxs-lookup"><span data-stu-id="95f23-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="95f23-107">عند الانتهاء، انقر فوق **حفظ التغييرات**.</span><span class="sxs-lookup"><span data-stu-id="95f23-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="95f23-108">في بعض الحالات، إذا تم تعيين الترخيص بالفعل إلى حساب مستخدم، فإن إزالة الترخيص ثم إعادة تعيينه يساعد على حل المشكلة وتوفيره بشكل صحيح في النظام:</span><span class="sxs-lookup"><span data-stu-id="95f23-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="95f23-109">تحقق لمعرفة ما إذا كانت اشتراكاتك في M365 Exchange Online (وغيرها، إذا كان لديك أي اشتراك) حالية ولم تنته صلاحيتها مؤخرا.</span><span class="sxs-lookup"><span data-stu-id="95f23-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="95f23-110">بعد التأكد من انتهاء صلاحية اشتراكك وتعيين ترخيص صالح لحساب المستخدم، قد يستغرق توفير الترخيص فترة تصل إلى 24 ساعة، لذا قد تحتاج إلى انتظار حل المشكلة.</span><span class="sxs-lookup"><span data-stu-id="95f23-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="95f23-111">لمزيد من المعلومات، راجع [تعيين التراخيص وإدارتها](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span><span class="sxs-lookup"><span data-stu-id="95f23-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>