---
title: الشروع في العمل مع SharePoint على الإنترنت
ms.author: pebaum
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: 4c0220dd2535a1ef41aeef99e2bfc3fe28bac03a
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36751659"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="35dda-102">مهام سير العمل في SharePoint</span><span class="sxs-lookup"><span data-stu-id="35dda-102">Workflows in SharePoint</span></span>

<span data-ttu-id="35dda-103">إذا لم تقم مهام سير عمل SharePoint بإرسال رسائل البريد الإلكتروني، فقد تكون مؤسستك قد واجهت حدود مرسل Exchange عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="35dda-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="35dda-104">قد تظهر رسالة الخطأ 'سير العمل مع وقف التنفيذ' إذا كان لديك أحد العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="35dda-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="35dda-105">لديك سير عمل في SharePoint على الإنترنت الذي يستخدم SharePoint 2010 أو SharePoint 2013 نوع النظام الأساسي لسير العمل.</span><span class="sxs-lookup"><span data-stu-id="35dda-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="35dda-106">تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة إلى أكثر من 200 مستخدم في كل مرة، أو أكثر من 10,000 مستلم في اليوم، أو أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="35dda-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="35dda-107">عند تشغيل سير العمل، لا يتم إرسال رسالة البريد الإلكتروني، وتلاحظ رسالة الخطأ، يتم تعيين "الحالة الداخلية" إلى "تعليق" أو "غير قادر على إرسال" إلى مستلم.</span><span class="sxs-lookup"><span data-stu-id="35dda-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="35dda-108">لمزيد من المعلومات، يرجى الرجوع إلى [المقالة](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)التالية .</span><span class="sxs-lookup"><span data-stu-id="35dda-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

