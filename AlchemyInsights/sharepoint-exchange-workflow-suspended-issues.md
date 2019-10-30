---
title: البدء باستخدام SharePoint علي الإنترنت
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
ms.openlocfilehash: 5e61491b626bfe75fd26a15ee54be82d9efa19a7
ms.sourcegitcommit: defe2c412567b596fa8c3ab52111bde712ebb314
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/29/2019
ms.locfileid: "37766878"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="ae474-102">مهام سير العمل في SharePoint</span><span class="sxs-lookup"><span data-stu-id="ae474-102">Workflows in SharePoint</span></span>

<span data-ttu-id="ae474-103">إذا لم يتم إرسال مهام سير عمل SharePoint رسائل البريد الكتروني ، قد واجهت مؤسستك حدود المرسل Exchange عبر إنترنت.</span><span class="sxs-lookup"><span data-stu-id="ae474-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="ae474-104">قد تظهر رسالة الخطا "سير العمل معلق" إذا كان لديك أحد العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="ae474-104">The 'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="ae474-105">لديك سير عمل في SharePoint علي الإنترنت التي تستخدم SharePoint 2010 أو SharePoint 2013 نوع النظام الأساسي سير العمل.</span><span class="sxs-lookup"><span data-stu-id="ae474-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="ae474-106">يتم تكوين سير العمل لإرسال رسالة بريد الكتروني مخصصه إلى أكثر من 200 المستخدمين في كل مره ، أكثر من 10,000 المستلمين في اليوم الواحد ، أو أكثر من 30 رسالة في الدقيقة الواحدة.</span><span class="sxs-lookup"><span data-stu-id="ae474-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="ae474-107">عند تشغيل سير العمل ، لا يتم إرسال رسالة البريد الكتروني ، ولاحظت رسالة الخطا ، يتم تعيين الحالة الداخلية إلى المعلقة أو غير قادر علي إرسال إلى مستلم يتم عرض.</span><span class="sxs-lookup"><span data-stu-id="ae474-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="ae474-108">لمزيد من المعلومات ، يرجى الرجوع إلى [المقالة](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running)التالية.</span><span class="sxs-lookup"><span data-stu-id="ae474-108">For more information, please refer to the following [article](https://docs.microsoft.com/sharepoint/support/workflows/configured-workflow-fails-running).</span></span>

