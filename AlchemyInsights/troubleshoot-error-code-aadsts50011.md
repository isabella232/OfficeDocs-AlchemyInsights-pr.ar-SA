---
title: استكشاف أخطاء رمز الخطأ AADSTS50011 وإصلاحها
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9802"
- "9005744"
ms.openlocfilehash: 6acf0ce3615669babd1a912ffd782b3750b93500
ms.sourcegitcommit: 1d73771d147325cfd8578e6816becd8331913890
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034865"
---
# <a name="troubleshoot-error-code-aadsts50011"></a><span data-ttu-id="456c2-102">استكشاف أخطاء رمز الخطأ AADSTS50011 وإصلاحها</span><span class="sxs-lookup"><span data-stu-id="456c2-102">Troubleshoot error code AADSTS50011</span></span>

<span data-ttu-id="456c2-103">لحل خطأ AADSTS50011، تنفيذ الخطوة الموصى بها الموضحة أدناه.</span><span class="sxs-lookup"><span data-stu-id="456c2-103">To resolve AADSTS50011 error, perform the recommended step described below.</span></span>

<span data-ttu-id="456c2-104">**AADSTS50011**: InvalidReplyTo - عنوان الرد مفقود أو غير مكون بشكل صحيح أو لا يطابق عناوين الرد التي تم تكوينها للتطبيق.</span><span class="sxs-lookup"><span data-stu-id="456c2-104">**AADSTS50011**: InvalidReplyTo - The reply address is missing, misconfigured, or does not match reply addresses configured for the app.</span></span>

<span data-ttu-id="456c2-105">كقرار، تأكد من إضافة عنوان الرد المفقود هذا إلى تطبيق Azure Active Directory (AD) أو أن يكون هناك شخص لديه الأذونات لإدارة التطبيق في AD للقيام بذلك من أجلك.</span><span class="sxs-lookup"><span data-stu-id="456c2-105">As a resolution ensure to add this missing reply address to the Azure Active Directory (AD) app or have someone with the permissions to manage your application in AD do this for you.</span></span> <span data-ttu-id="456c2-106">لمزيد من المعلومات، راجع مقالة استكشاف الأخطاء وإصلاحها للخطأ [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span><span class="sxs-lookup"><span data-stu-id="456c2-106">For more information, see the troubleshooting article for error [AADSTS50011](https://docs.microsoft.com/troubleshoot/azure/active-directory/error-code-aadsts50011-reply-url-mismatch).</span></span>