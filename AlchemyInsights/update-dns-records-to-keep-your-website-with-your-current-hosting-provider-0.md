---
title: تحديث سجلات DNS لإبقاء موقعك على ويب مع موفر الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 89bce2aa5931c0c20706efabd42d2351be43938b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827492"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="976c2-102">تحديث سجلات DNS لإبقاء موقعك على ويب مع موفر الاستضافة الحالي</span><span class="sxs-lookup"><span data-stu-id="976c2-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="976c2-103">في مركز إدارة Microsoft 365، انتقل إلى صفحة مجالات الإعداد، وفي قائمة المجالات، حدد المجال الذي تستخدمه  >  [](https://admin.microsoft.com/Adminportal#/Domains) لموقعك على ويب.</span><span class="sxs-lookup"><span data-stu-id="976c2-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="976c2-104">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="976c2-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="976c2-105">بالنسبة **لنوع DNS،** أدخل: **أ (عنوان)**</span><span class="sxs-lookup"><span data-stu-id="976c2-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="976c2-106">بالنسبة **إلى اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **@**</span><span class="sxs-lookup"><span data-stu-id="976c2-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="976c2-107">بالنسبة **إلى عنوان IP**، اكتب عنوان IP الثابت لموقعك على ويب حيث يستضيفه حاليا (على سبيل المثال، 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="976c2-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="976c2-108">يجب أن يكون  *هذا عنوان*  IP ثابتا لموقع ويب، وليس  *عنوان*  IP ديناميكيا.</span><span class="sxs-lookup"><span data-stu-id="976c2-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="976c2-109">تحقق من الموقع الذي يستضيف موقعك على ويب للتأكد من أنه يمكنك الحصول على عنوان IP ثابت لموقعك العام على ويب.</span><span class="sxs-lookup"><span data-stu-id="976c2-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="976c2-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="976c2-110">Select **Save**.</span></span>

<span data-ttu-id="976c2-111">بالإضافة إلى ذلك، يمكنك إنشاء سجل CNAME لمساعدة العملاء في العثور على موقعك على ويب.</span><span class="sxs-lookup"><span data-stu-id="976c2-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="976c2-112">حدد **+ سجل مخصص جديد** وأدخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="976c2-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="976c2-113">بالنسبة **لنوع DNS،** أدخل: **CNAME (الاسم المستعار)**</span><span class="sxs-lookup"><span data-stu-id="976c2-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="976c2-114">بالنسبة **إلى اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **www**</span><span class="sxs-lookup"><span data-stu-id="976c2-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="976c2-115">لنقاط **العنوان**، اكتب اسم المجال المؤهل بالكامل (FQDN) لموقعك على ويب (على سبيل المثال، contoso.com).</span><span class="sxs-lookup"><span data-stu-id="976c2-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="976c2-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="976c2-116">Select **Save**.</span></span>
