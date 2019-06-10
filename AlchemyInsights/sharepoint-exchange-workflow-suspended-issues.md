---
title: الشروع في استخدام SharePoint على الإنترنت
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 7ae05f21-eb16-4d71-9e19-4f097eb100d2
ms.openlocfilehash: afb1ef115d364ee3e2cf09ea850adb57ad1d44e6
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770550"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="72fc4-102">مهام سير العمل في SharePoint</span><span class="sxs-lookup"><span data-stu-id="72fc4-102">Workflows in SharePoint</span></span>

<span data-ttu-id="72fc4-103">إذا كانت مهام سير العمل SharePoint لا ترسل رسائل البريد الإلكتروني، قد واجهت المؤسسة حدود المرسل Exchange عبر إنترنت.</span><span class="sxs-lookup"><span data-stu-id="72fc4-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.</span></span>

<span data-ttu-id="72fc4-104">قد تظهر رسالة الخطأ 'تم تعليق سير العمل' إذا كان لديك أحد العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="72fc4-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span>

- <span data-ttu-id="72fc4-105">يكون سير عمل في SharePoint على الإنترنت الذي يستخدم SharePoint 2010 أو نوع النظام الأساسي لسير العمل SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="72fc4-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>

- <span data-ttu-id="72fc4-106">تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة للمستخدمين أكثر من 200 في مرة الواحدة أو المستلمين أكثر من 10 آلاف يوميا أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="72fc4-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>

<span data-ttu-id="72fc4-107">عند تشغيل سير العمل وعدم إرسال رسالة البريد الإلكتروني وتلاحظ رسالة الخطأ، يتم تعيين "حالة داخلية" عرض معلق أو تعذرت لإرسال إلى مستلم.</span><span class="sxs-lookup"><span data-stu-id="72fc4-107">When you run the workflow, the email message isn't sent, and you notice the error message, Internal Status is set to Suspended or Unable to send to a recipient is displayed.</span></span>

<span data-ttu-id="72fc4-108">لمزيد من المعلومات، الرجاء الرجوع إلى [المقالة](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US)التالية.</span><span class="sxs-lookup"><span data-stu-id="72fc4-108">For more information, please refer to the following [article](https://support.office.com/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

