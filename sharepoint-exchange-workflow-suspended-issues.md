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
ms.openlocfilehash: 9a8d72a01ed35794fcab370b48bbb189663d3396
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/04/2019
ms.locfileid: "34718734"
---
# <a name="workflows-in-sharepoint"></a><span data-ttu-id="d07af-102">مهام سير العمل في SharePoint</span><span class="sxs-lookup"><span data-stu-id="d07af-102">Workflows in SharePoint</span></span>

<p><span data-ttu-id="d07af-103">إذا كانت مهام سير العمل SharePoint لا ترسل رسائل البريد الإلكتروني، قد واجهت المؤسسة حدود المرسل Exchange عبر إنترنت.&nbsp;</span><span class="sxs-lookup"><span data-stu-id="d07af-103">If SharePoint workflows are not sending emails, your organization may have encountered the Exchange Online sender limits.&nbsp;</span></span></p> <p><span data-ttu-id="d07af-104">قد تظهر رسالة الخطأ 'تم تعليق سير العمل' إذا كان لديك أحد العناصر التالية:</span><span class="sxs-lookup"><span data-stu-id="d07af-104">'Workflow is Suspended' error message may occur if you have one of the following items:</span></span></p> <ul> <li><span data-ttu-id="d07af-105">يكون سير عمل في SharePoint على الإنترنت الذي يستخدم SharePoint 2010 أو نوع النظام الأساسي لسير العمل SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="d07af-105">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span></li> <li><span data-ttu-id="d07af-106">تم تكوين سير العمل لإرسال رسالة بريد إلكتروني مخصصة للمستخدمين أكثر من 200 في مرة الواحدة أو المستلمين أكثر من 10 آلاف يوميا أكثر من 30 رسالة في الدقيقة.</span><span class="sxs-lookup"><span data-stu-id="d07af-106">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span></li> <li><span data-ttu-id="d07af-107">عندما تقوم بتشغيل سير العمل وعدم إرسال رسالة البريد الإلكتروني ولاحظت رسالة الإعلام بالخطأ، يتم عرض <strong>"الحالة الداخلية" معينة إلى معلق</strong> أو <strong>لا يمكن إرسال إلى مستلم</strong> .</span><span class="sxs-lookup"><span data-stu-id="d07af-107">When you run the workflow, the email message isn't sent, and you notice the error message, <strong>Internal Status is set to Suspended</strong> or <strong>Unable to send to a recipient</strong> is displayed.</span></span></li> </ul> <p><span data-ttu-id="d07af-108">لمزيد من المعلومات، الرجاء الرجوع إلى <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">المقالة</a>التالية.</span><span class="sxs-lookup"><span data-stu-id="d07af-108">For more information, please refer to the following <a href="https://support.office.com/en-us/article/-daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or-unable-to-send-to-a-recipient-error-in-a-sharepoint-online-workflow-89d02169-5fa6-4259-affc-73edb6ca9fb6?ui=en-US&amp;rs=en-US&amp;ad=US">article</a>.</span></span></p>

