---
title: تحديث خوادم أسماء المجال للإشارة إلى Microsoft
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 5d38b331-a0e8-4937-8bda-4f8f715e1976
ms.custom:
- "6"
- "14"
ms.openlocfilehash: b49ca9422f582f906fc6c108c85cc26150474548
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719980"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="ab746-102">تحديث خوادم أسماء المجال للإشارة إلى Microsoft</span><span class="sxs-lookup"><span data-stu-id="ab746-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="ab746-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="ab746-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="ab746-104">لإعداد نطاقك مع Microsoft، يجب تحديث خوادم الأسماء في المسجل.</span><span class="sxs-lookup"><span data-stu-id="ab746-104">To set up your domain with Microsoft, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="ab746-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="ab746-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="ab746-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="ab746-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="ab746-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="ab746-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="ab746-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ab746-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="ab746-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="ab746-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="ab746-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="ab746-110">Save changes.</span></span>

<span data-ttu-id="ab746-111">يمكنك أيضًا العثور على إرشادات تفصيلية في هذه المقالة: [تغيير خوادم الأسماء لإعداد Microsoft 365 مع أي مسجل نطاق](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="ab746-111">You can also find detailed instructions in this article: [Change nameservers to set up Microsoft 365 with any domain registrar](https://docs.microsoft.com/office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  