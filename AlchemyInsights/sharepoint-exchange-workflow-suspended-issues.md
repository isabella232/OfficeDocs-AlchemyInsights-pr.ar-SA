---
title: بدء استخدام SharePoint Online
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: bba89489cb75555e1f508224de223bee04e1d665
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700694"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="83540-102">مهام سير العمل في SharePoint</span><span class="sxs-lookup"><span data-stu-id="83540-102">Workflows in SharePoint</span></span>

<span data-ttu-id="83540-103">إذا لم ترسل مهام سير عمل SharePoint رسائل البريد الكتروني ، فقد تكون مؤسستك واجهت حدود مرسل Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="83540-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="83540-104">قد تظهر رسالة الخطا "توقف سير العمل مرحليا" إذا كان لديك أحد العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="83540-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="83540-105">لديك سير عمل في SharePoint Online يستخدم نوع النظام الأساسي لسير العمل SharePoint 2010 أو SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="83540-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="83540-106">تم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 مستخدمين في نفس الوقت ، أو أكثر من 10,000 مستلم في اليوم ، أو أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="83540-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="83540-107">عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، وتلاحظ ظهور رسالة الخطا ، يتم تعيين الحالة الداخلية إلى معلق أو تعذر الإرسال إلى المستلم.</span><span class="sxs-lookup"><span data-stu-id="83540-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="83540-108">لمزيد من المعلومات ، يرجى مراجعه [المقالة](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)التالية.</span><span class="sxs-lookup"><span data-stu-id="83540-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

