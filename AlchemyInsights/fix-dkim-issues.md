---
title: إصلاح مشكلات إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717549"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="0b6a8-102">إصلاح مشكلات إعداد DKIM</span><span class="sxs-lookup"><span data-stu-id="0b6a8-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="0b6a8-103">إذا واجهت مشكلات تمكين DKIM للمجال المخصص الخاص بك، استخدم الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0b6a8-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="0b6a8-104">ترتبط معظم مشكلات إعداد DKIM بسجلات DNS غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="0b6a8-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="0b6a8-105">تحقق من تنسيق سجل DKIM CNAME **(وليس** سجل TXT) بشكل صحيح.</span><span class="sxs-lookup"><span data-stu-id="0b6a8-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="0b6a8-106">لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="0b6a8-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="0b6a8-107">بعد إنشاء سجلات Dns DKIM أو تحديثها في خدمة استضافة DNS لنطاقك (عادةً، مسجل النطاق الخاص بك)، انتظر حتى تنتشر سجلات DNS.</span><span class="sxs-lookup"><span data-stu-id="0b6a8-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="0b6a8-108">إذا لم تتمكن من إنشاء سجلات Dns DKIM في \<مركز\> المسؤول، يمكنك استبدال CustomDomain بالمجال المخصص (على سبيل `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`المثال، contoso.com) وتشغيل هذا الأمر في Exchange Online [PowerShell:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="0b6a8-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
