---
title: تغيير خوادم الأسماء
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 572f8befd84f55cb07a3535852a46e735d3ed620
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706742"
---
# <a name="update-your-domain-nameservers-to-point-to-microsoft"></a><span data-ttu-id="16e10-102">تحديث خوادم أسماء المجال للإشارة إلى Microsoft</span><span class="sxs-lookup"><span data-stu-id="16e10-102">Update your domain nameservers to point to Microsoft</span></span>

<span data-ttu-id="16e10-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="16e10-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="16e10-104">لإعداد مجالك في Microsoft 365، يجب تحديث خوادم الأسماء لدى جهة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="16e10-104">To set up your domain in Microsoft 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="16e10-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="16e10-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="16e10-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="16e10-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="16e10-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="16e10-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="16e10-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="16e10-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="16e10-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="16e10-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="16e10-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="16e10-110">Save changes.</span></span>

<span data-ttu-id="16e10-111">يمكنك أيضاً العثور على إرشادات مفصلة في هذه المقالة: [تغيير أسماء الخوادم لدى أي جهة تسجيل المجالات](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="16e10-111">You can also find detailed instructions in this article: [Change nameservers with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  