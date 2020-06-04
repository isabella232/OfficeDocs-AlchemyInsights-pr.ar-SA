---
title: تحديث سجلات DNS للحفاظ على موقعك على الويب مع مزود الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665747"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="16b74-102">تحديث سجلات DNS للحفاظ على موقعك على الويب مع مزود الاستضافة الحالي</span><span class="sxs-lookup"><span data-stu-id="16b74-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="16b74-103">في مركز إدارة Microsoft 365، **Setup**انتقل إلى صفحة  >  [نطاقات](https://portal.office.com/adminportal/home#/Domains) الإعداد، وفي قائمة المجالات، حدد المجال الذي تستخدمه لموقعك على الويب.</span><span class="sxs-lookup"><span data-stu-id="16b74-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://portal.office.com/adminportal/home#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="16b74-104">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="16b74-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="16b74-105">لإدخال **نوع DNS:** **أ (عنوان)**</span><span class="sxs-lookup"><span data-stu-id="16b74-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="16b74-106">لاسم **المضيف أو الاسم المستعار**، اكتب ما يلي:**@**</span><span class="sxs-lookup"><span data-stu-id="16b74-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="16b74-107">بالنسبة **إلى عنوان IP**، اكتب عنوان IP الثابت لموقع الويب الخاص بك حيث يتم استضافته حاليًا (على سبيل المثال ، 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="16b74-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="16b74-108">يجب أن يكون هذا عنوان IP *ثابت* لموقع الويب، وليس عنوان IP *ديناميكي.*</span><span class="sxs-lookup"><span data-stu-id="16b74-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="16b74-109">تحقق مع الموقع الذي يتم فيه استضافة موقع الويب الخاص بك للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقعك العام.</span><span class="sxs-lookup"><span data-stu-id="16b74-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="16b74-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="16b74-110">Select **Save**.</span></span>

<span data-ttu-id="16b74-111">بالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء في العثور على موقعك على الويب.</span><span class="sxs-lookup"><span data-stu-id="16b74-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="16b74-112">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="16b74-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="16b74-113">لإدخال **نوع DNS:** **CNAME (الاسم المستعار)**</span><span class="sxs-lookup"><span data-stu-id="16b74-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="16b74-114">لاسم **المضيف أو الاسم المستعار،** اكتب ما يلي: **www**</span><span class="sxs-lookup"><span data-stu-id="16b74-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="16b74-115">للحصول **على نقاط للعنوان**، اكتب اسم النطاق المؤهل بالكامل (FQDN) لموقعك على الويب (على سبيل المثال ، contoso.com).</span><span class="sxs-lookup"><span data-stu-id="16b74-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="16b74-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="16b74-116">Select **Save**.</span></span>
