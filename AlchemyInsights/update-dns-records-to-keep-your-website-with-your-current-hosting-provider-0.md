---
title: تحديث سجلات DNS للحفاظ على موقع الويب الخاص بك باستخدام موفر الاستضافة الحالية
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: e437015d476c1417fa37e1b1c250e2205e9ce4d9
ms.sourcegitcommit: b825ced7b66d452b0f3874a57e033e690ec41c93
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/29/2019
ms.locfileid: "35925272"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="a7ec1-102">تحديث سجلات DNS للحفاظ على موقع الويب الخاص بك باستخدام موفر الاستضافة الحالية</span><span class="sxs-lookup"><span data-stu-id="a7ec1-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="a7ec1-103">على الصفحة " [مجالات](https://portal.office.com/adminportal/home#/Domains) "، في قائمة المجالات، حدد المجال الذي تستخدمه لموقع الويب الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a7ec1-103">On the [Domains](https://portal.office.com/adminportal/home#/Domains) page, in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="a7ec1-104">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="a7ec1-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a7ec1-105">أدخل نوع **DNS** : **(عنوان)**</span><span class="sxs-lookup"><span data-stu-id="a7ec1-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="a7ec1-106">**اسم المضيف أو اسم مستعار**، اكتب ما يلي:**@**</span><span class="sxs-lookup"><span data-stu-id="a7ec1-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="a7ec1-107">**عنوان IP**، اكتب عنوان IP لموقع الويب الخاص بك حيث يتم حاليا استضافته (على سبيل المثال، 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="a7ec1-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="a7ec1-108">يجب أن يكون عنوان IP *ثابت* لموقع ويب، وليس عنوان IP *حيوي* .</span><span class="sxs-lookup"><span data-stu-id="a7ec1-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="a7ec1-109">تحقق من الموقع حيث استضافة موقع الويب الخاص بك للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقع الويب العمومي الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a7ec1-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="a7ec1-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a7ec1-110">Select **Save**.</span></span>

<span data-ttu-id="a7ec1-111">وبالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء على العثور على موقع الويب الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="a7ec1-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="a7ec1-112">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="a7ec1-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="a7ec1-113">أدخل نوع **DNS** : **CNAME (اسم مستعار)**</span><span class="sxs-lookup"><span data-stu-id="a7ec1-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="a7ec1-114">**اسم المضيف أو اسم مستعار**، اكتب ما يلي: **www**</span><span class="sxs-lookup"><span data-stu-id="a7ec1-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="a7ec1-115">**يشير إلى عنوان**، اكتب اسم المجال المؤهل بالكامل (FQDN) لموقع الويب الخاص بك (على سبيل المثال، "contoso.com" أيضا).</span><span class="sxs-lookup"><span data-stu-id="a7ec1-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="a7ec1-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="a7ec1-116">Select **Save**.</span></span>
