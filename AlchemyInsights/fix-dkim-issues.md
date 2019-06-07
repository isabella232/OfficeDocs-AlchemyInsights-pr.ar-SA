---
title: إصلاح مشكلات إعداد DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: 4d6dadbcbf71fe6e9ea56d6a82a7d8ababdd38ef
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764801"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="c8cec-102">إصلاح مشكلات إعداد DKIM</span><span class="sxs-lookup"><span data-stu-id="c8cec-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="c8cec-103">إذا واجهت مشكلات تمكين DKIM للمجال المخصص الخاص بك، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c8cec-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="c8cec-104">ترتبط معظم مشاكل الإعداد DKIM سجلات DNS غير صحيحة.</span><span class="sxs-lookup"><span data-stu-id="c8cec-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="c8cec-105">تحقق من تنسيق سجل DKIM CNAME (**لا** سجل TXT).</span><span class="sxs-lookup"><span data-stu-id="c8cec-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="c8cec-106">لمزيد من المعلومات، راجع هذا [الموضوع](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="c8cec-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="c8cec-107">بعد أن تقوم بإنشاء أو تحديث سجلات DKIM DNS في DNS المجان للمجال الخاص بك (بشكل عام، مسجل النطاق)، انتظر حتى يتم نشر سجلات DNS.</span><span class="sxs-lookup"><span data-stu-id="c8cec-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="c8cec-108">إذا لا يمكن إنشاء سجلات DKIM DNS في مركز مسؤول، يمكنك استبدال \<كوستومدومين\> مع المجال المخصص الخاص بك (على سبيل المثال، contoso.com) وتشغيل هذا الأمر في [PowerShell Exchange الفورية](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span><span class="sxs-lookup"><span data-stu-id="c8cec-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
