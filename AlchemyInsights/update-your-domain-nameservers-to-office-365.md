---
title: تحديث خوادم أسماء المجال إلى Office 365
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 5/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: 23d49c734148739ede0d5e5b53430a42b606c831
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36742145"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="3ec95-102">تحديث خوادم أسماء المجال إلى Office 365</span><span class="sxs-lookup"><span data-stu-id="3ec95-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="3ec95-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="3ec95-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3ec95-104">لإعداد مجالك في Office 365، يجب تحديث خوادم الأسماء لدى جهة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="3ec95-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="3ec95-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="3ec95-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3ec95-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="3ec95-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="3ec95-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="3ec95-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3ec95-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3ec95-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3ec95-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3ec95-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3ec95-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="3ec95-110">Save changes.</span></span>

<span data-ttu-id="3ec95-111">يمكنك أيضاً العثور على إرشادات مفصلة في هذه المقالة: [تغيير أسماء الخوادم لإعداد Office 365 لدى أي جهة تسجيل مجالات](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="3ec95-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  