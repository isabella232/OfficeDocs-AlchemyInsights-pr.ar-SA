---
title: الإرسال كمجلد عام ممكن علي البريد في أكسو
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461735"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="f76a9-102">سندس المجلد العام الممكن للبريد</span><span class="sxs-lookup"><span data-stu-id="f76a9-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="f76a9-103">يعين المثال التالي الأذونات "إرسال ك" لNewPF1 المجلدات العمومية الممكنة للبريد لجيسون المستخدم.</span><span class="sxs-lookup"><span data-stu-id="f76a9-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="f76a9-104">Add-RecipientPermission-Identity NewPF1-الجهة الموثوق بها "جيسون"-أكسيسريغتس ' سينداس '</span><span class="sxs-lookup"><span data-stu-id="f76a9-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="f76a9-105">بالنسبة إلى بناء الجملة ومعلومات المعلمات التفصيلية ، راجع [تعيين أذونات "إرسال ك" أو "إرسال بالنيابة عن" للمجلدات العمومية الممكنة للبريد](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="f76a9-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

