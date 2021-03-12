---
title: إصلاح المشاكل الشائعة في تنسيق سجل DKIM
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 0a59ca1c93121cb4681c0d44b85a9b756c07895b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743407"
---
# <a name="fix-common-problems-with-dkim-record-formatting"></a><span data-ttu-id="2e35c-102">إصلاح المشاكل الشائعة في تنسيق سجل DKIM</span><span class="sxs-lookup"><span data-stu-id="2e35c-102">Fix common problems with DKIM record formatting</span></span>

<span data-ttu-id="2e35c-103">ترتبط معظم مشاكل إعداد DKIM بسجلات DNS غير الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="2e35c-103">Most DKIM set-up issues are related to incorrect DNS records.</span></span>

<span data-ttu-id="2e35c-104">لإصلاح مشاكل إعداد DKIM، تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="2e35c-104">To fix the DKIM set-up issues, verify that the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="2e35c-105">لمزيد من المعلومات، راجع ما يجب فعله لإعداد [DKIM يدويا في Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span><span class="sxs-lookup"><span data-stu-id="2e35c-105">For more information, see [What you need to do to manually set up DKIM in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email).</span></span>

<span data-ttu-id="2e35c-106">إذا كنت بحاجة إلى مساعدة في سجلات DNS بشكل عام، فشاهد إنشاء [سجلات DNS لدى أي موفر استضافة DNS ل Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="2e35c-106">If you need help with DNS records in general, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>

> [!NOTE]
> <span data-ttu-id="2e35c-107">بعد إنشاء سجلات DNS DKIM أو تحديثها في خدمة استضافة DNS لمجالك، ستحتاج إلى انتظار نشر سجلات DNS.</span><span class="sxs-lookup"><span data-stu-id="2e35c-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain, you'll need to wait for the DNS records to propagate.</span></span>
