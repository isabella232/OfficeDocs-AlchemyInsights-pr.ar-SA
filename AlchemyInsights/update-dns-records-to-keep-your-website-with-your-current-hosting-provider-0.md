---
title: تحديث سجلات DNS للاحتفاظ بموقعك علي ويب مع موفر الاستضافة الحالي
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 1d8654bc2dfb9063d0203992d624285eb646027d
ms.sourcegitcommit: 78939b01579b626b147d356045a37aec1170c948
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47815772"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a><span data-ttu-id="1e567-102">تحديث سجلات DNS للاحتفاظ بموقعك علي ويب مع موفر الاستضافة الحالي</span><span class="sxs-lookup"><span data-stu-id="1e567-102">Update DNS records to keep your website with your current hosting provider</span></span>

1. <span data-ttu-id="1e567-103">في مركز أداره Microsoft 365 ، انتقل إلى صفحه **"إعدادات**  >  [المجالات](https://admin.microsoft.com/Adminportal#/Domains) " ، وفي قائمه المجالات ، حدد المجال الذي تستخدمه لموقعك علي ويب.</span><span class="sxs-lookup"><span data-stu-id="1e567-103">In the Microsoft 365 admin center, go to the **Setup** > [Domains](https://admin.microsoft.com/Adminportal#/Domains) page, and in the list of domains, select the domain you're using for your website.</span></span>

2. <span data-ttu-id="1e567-104">**حدد + سجل مخصص جديد** وادخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="1e567-104">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1e567-105">بالنسبة إلى **نوع DNS** ، ادخل: **(عنوان)**</span><span class="sxs-lookup"><span data-stu-id="1e567-105">For **DNS type** enter: **A (Address)**</span></span>

  - <span data-ttu-id="1e567-106">بالنسبة إلى **اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **@**</span><span class="sxs-lookup"><span data-stu-id="1e567-106">For **Host name or Alias**, type the following: **@**</span></span>

  - <span data-ttu-id="1e567-107">بالنسبة إلى **عنوان ip**، اكتب عنوان ip الثابت لموقع ويب الخاص بك حيث تتم استضافته حاليا (علي سبيل المثال ،: 172.16.140.1).</span><span class="sxs-lookup"><span data-stu-id="1e567-107">For **IP Address**, type the static IP address for your website where it's currently hosted (for example, 172.16.140.1).</span></span>

    <span data-ttu-id="1e567-108">يجب ان يكون هذا عنوان ip  *ثابتا*  لموقع ويب ، وليس عنوان ip  *ديناميكي*  .</span><span class="sxs-lookup"><span data-stu-id="1e567-108">This must be a  *static*  IP address for the website, not a  *dynamic*  IP address.</span></span> <span data-ttu-id="1e567-109">راجع الموقع حيث تتم استضافه موقعك علي ويب للتاكد من انه يمكنك الحصول علي عنوان IP ثابت لموقعك العام علي ويب.</span><span class="sxs-lookup"><span data-stu-id="1e567-109">Check with site where your website is hosted to make sure you can get a static IP address for your public website.</span></span>

3. <span data-ttu-id="1e567-110">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1e567-110">Select **Save**.</span></span>

<span data-ttu-id="1e567-111">بالاضافه إلى ذلك ، يمكنك إنشاء سجل CNAME لمساعده العملاء علي العثور علي موقعك علي ويب.</span><span class="sxs-lookup"><span data-stu-id="1e567-111">In addition, you can create a CNAME record to help customers find your website.</span></span>
  
1. <span data-ttu-id="1e567-112">**حدد + سجل مخصص جديد** وادخل ما يلي:</span><span class="sxs-lookup"><span data-stu-id="1e567-112">Select **+ New custom record** and enter the following:</span></span>

  - <span data-ttu-id="1e567-113">بالنسبة إلى **نوع DNS** الإدخال: **CNAME (Alias)**</span><span class="sxs-lookup"><span data-stu-id="1e567-113">For **DNS type** enter: **CNAME (Alias)**</span></span>

  - <span data-ttu-id="1e567-114">بالنسبة إلى **اسم المضيف أو الاسم المستعار**، اكتب ما يلي: **www**</span><span class="sxs-lookup"><span data-stu-id="1e567-114">For **Host name or Alias**, type the following: **www**</span></span>

  - <span data-ttu-id="1e567-115">بالنسبة **إلى العنوان**، اكتب اسم المجال المؤهل بالبالكامل (FQDN) لموقعك علي ويب (علي سبيل المثال ، contoso.com).</span><span class="sxs-lookup"><span data-stu-id="1e567-115">For **Points to address**, type the fully qualified domain name (FQDN) for your website (for example, contoso.com).</span></span>

2. <span data-ttu-id="1e567-116">حدد **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="1e567-116">Select **Save**.</span></span>
