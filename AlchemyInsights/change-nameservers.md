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
ms.openlocfilehash: f4b5001f2a6291a422b5cd0c3c40de7be0f1ecf0
ms.sourcegitcommit: 20b6a1fb3f0d899f3b204e3c066262d10623a4ea
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/25/2019
ms.locfileid: "35902916"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="b0b4c-102">تحديث خوادم أسماء المجال إلى Office 365</span><span class="sxs-lookup"><span data-stu-id="b0b4c-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="b0b4c-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="b0b4c-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="b0b4c-104">لإعداد مجالك في Office 365، يجب تحديث خوادم الأسماء لدى جهة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="b0b4c-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="b0b4c-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="b0b4c-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="b0b4c-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="b0b4c-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>
  
2. <span data-ttu-id="b0b4c-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="b0b4c-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="b0b4c-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b0b4c-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="b0b4c-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b0b4c-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="b0b4c-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="b0b4c-110">Save changes.</span></span>

<span data-ttu-id="b0b4c-111">يمكنك أيضاً العثور على إرشادات مفصلة في هذه المقالة: [تغيير أسماء الخوادم لإعداد Office 365 لدى أي جهة تسجيل مجالات](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="b0b4c-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  