---
title: تغيير خوادم الأسماء
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5"
- "14"
ms.openlocfilehash: 51532f42e7cbd39ebad3f0160465218c6e1454a2
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36736636"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="7252c-102">تحديث خوادم أسماء المجال إلى Office 365</span><span class="sxs-lookup"><span data-stu-id="7252c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="7252c-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="7252c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="7252c-104">لإعداد مجالك في Office 365، يجب تحديث خوادم الأسماء لدى جهة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="7252c-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="7252c-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="7252c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="7252c-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="7252c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="7252c-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="7252c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="7252c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7252c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="7252c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="7252c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="7252c-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="7252c-110">Save changes.</span></span>

<span data-ttu-id="7252c-111">يمكنك أيضاً العثور على إرشادات مفصلة في هذه المقالة: [تغيير أسماء الخوادم لإعداد Office 365 لدى أي جهة تسجيل مجالات](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span><span class="sxs-lookup"><span data-stu-id="7252c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://docs.microsoft.com//office365/admin/get-help-with-domains/change-nameservers-at-any-domain-registrar)</span></span>
  