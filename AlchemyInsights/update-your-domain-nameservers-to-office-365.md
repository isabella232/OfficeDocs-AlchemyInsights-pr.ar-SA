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
ms.openlocfilehash: 8e25c510233f2a00d133ea69a338141c5a475465
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35352876"
---
# <a name="update-your-domain-nameservers-to-office-365"></a><span data-ttu-id="3cbbc-102">تحديث خوادم أسماء المجال إلى Office 365</span><span class="sxs-lookup"><span data-stu-id="3cbbc-102">Update your domain nameservers to Office 365</span></span>

<span data-ttu-id="3cbbc-103">ملاحظة: قد تستغرق تغييرات خادم الأسماء أحياناً ما يصل إلى 48 ساعة ليتم نشرها.</span><span class="sxs-lookup"><span data-stu-id="3cbbc-103">Note: Nameserver changes can sometimes take up to 48 hours to propagate.</span></span>
  
<span data-ttu-id="3cbbc-104">لإعداد مجالك في Office 365، يجب تحديث خوادم الأسماء لدى جهة التسجيل.</span><span class="sxs-lookup"><span data-stu-id="3cbbc-104">To set up your domain in Office 365, the nameservers at your registrar need to be updated.</span></span> <span data-ttu-id="3cbbc-105">إنشاء سجلات خادم الأسماء أو تحريرها لدى جهة تسجيل المجالات.</span><span class="sxs-lookup"><span data-stu-id="3cbbc-105">Create or edit your nameserver records at your domain registrar.</span></span>
  
1. <span data-ttu-id="3cbbc-106">انتقل إلى موقع جهة تسجيل المجالات على ويب وابحث عن المنطقة التي يمكنك فيها تحرير خوادم الأسماء.</span><span class="sxs-lookup"><span data-stu-id="3cbbc-106">Go to your domain registrar's website and find the area where you can edit the nameservers.</span></span>

2. <span data-ttu-id="3cbbc-107">إنشاء اثنين من سجلات خادم الأسماء أو تحريرها لتتطابق مع هذه القيم:</span><span class="sxs-lookup"><span data-stu-id="3cbbc-107">Create or edit two nameserver records to match these values:</span></span>

  - <span data-ttu-id="3cbbc-108">ns1.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3cbbc-108">ns1.bdm.microsoftonline.com</span></span>

  - <span data-ttu-id="3cbbc-109">ns2.bdm.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="3cbbc-109">ns2.bdm.microsoftonline.com</span></span>

3. <span data-ttu-id="3cbbc-110">حفظ التغييرات.</span><span class="sxs-lookup"><span data-stu-id="3cbbc-110">Save changes.</span></span>

<span data-ttu-id="3cbbc-111">يمكنك أيضاً العثور على إرشادات مفصلة في هذه المقالة: [تغيير أسماء الخوادم لإعداد Office 365 لدى أي جهة تسجيل مجالات](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span><span class="sxs-lookup"><span data-stu-id="3cbbc-111">You can also find detailed instructions in this article: [Change nameservers to set up Office 365 with any domain registrar](https://support.office.com/article/Change-nameservers-at-any-domain-registrar-to-set-up-Office-365-a8b487a9-2a45-4581-9dc4-5d28a47010a2.aspx)</span></span>
  