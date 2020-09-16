---
title: إصلاح مشاكل اعداد الأشرف
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 35e8023d26fe26211e27521ceb8751d2d7fc7a21
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47744937"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="69727-102">إصلاح مشاكل اعداد الأشرف</span><span class="sxs-lookup"><span data-stu-id="69727-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="69727-103">إذا واجهت مشاكل في تمكين DKIM لمجالك المخصص ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="69727-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="69727-104">ترتبط معظم مشاكل اعداد DKIM بسجلات DNS غير الصحيحة.</span><span class="sxs-lookup"><span data-stu-id="69727-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="69727-105">تاكد من تنسيق السجل الخاص ب DKIM CNAME (**وليس** سجل TXT) بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="69727-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="69727-106">لمزيد من المعلومات ، راجع هذا [الموضوع](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span><span class="sxs-lookup"><span data-stu-id="69727-106">For more information, see this [topic](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).</span></span>

- <span data-ttu-id="69727-107">بعد إنشاء سجلات DNS الخاصة ب DKIM أو تحديثها في خدمه استضافه DNS لمجالك (عاده ما يكون جهة تسجيل المجالات الخاصة بك) ، انتظر حتى يتم نشر سجلات DNS.</span><span class="sxs-lookup"><span data-stu-id="69727-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="69727-108">إذا لم تتمكن من إنشاء سجلات DNS ل DKIM في مركز الاداره ، فيمكنك استبدالها \<CustomDomain\> بمجالك المخصص (علي سبيل المثال ، contoso.com) وتشغيل هذا الأمر في [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true` .</span><span class="sxs-lookup"><span data-stu-id="69727-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
