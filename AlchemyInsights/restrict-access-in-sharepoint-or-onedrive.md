---
title: تقييد الوصول في SharePoint أو أندريف
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551438"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="77d94-102">تقييد الوصول في SharePoint أو أندريف</span><span class="sxs-lookup"><span data-stu-id="77d94-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="77d94-103">في SharePoint وأونيدريفي، يمكنك تقييد الوصول إلى عناصر مثل الملفات والمجلدات وقوائم بمنح حق الوصول فقط إلى المجموعات أو الأفراد بحق.</span><span class="sxs-lookup"><span data-stu-id="77d94-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="77d94-104">بشكل افتراضي، يتم توريث الأذونات في SharePoint من أعلى أعلى في التسلسل الهرمي.</span><span class="sxs-lookup"><span data-stu-id="77d94-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="77d94-105">لذا ملف يرث أذوناته من المجلد يرث أذوناته من المكتبة، يرث أذوناته من الموقع.</span><span class="sxs-lookup"><span data-stu-id="77d94-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="77d94-106">يمكنك مشاركة على مستوى أعلى (مثل بمشاركة موقع بأكمله) وبعد ذلك قطع التوريث إذا لم ترغب في مشاركة كافة العناصر الموجودة في الموقع.</span><span class="sxs-lookup"><span data-stu-id="77d94-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="77d94-107">ومع ذلك، لا نوصي هذا لأنه يجعل الحفاظ على الأذونات أكثر تعقيداً واضطراب في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="77d94-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="77d94-108">هنا ما الذي يمكن أن تفعله بدلاً من ذلك:</span><span class="sxs-lookup"><span data-stu-id="77d94-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="77d94-109">إذا، على سبيل المثال، تريد مشاركة كافة محتويات المجلد باستثناء ملف واحد في ذلك، نقل هذا الملف إلى موقع جديد غير المشتركة.</span><span class="sxs-lookup"><span data-stu-id="77d94-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="77d94-110">إذا كان لديك اثنين من المجلدات الفرعية في مجلد، وتريد مشاركة مجلد فرعي واحد مع المجموعات ألف وباء والسماح بوصول المجموعة الأولى فقط إلى المجلد الفرعي الثاني ومشاركة المجلد الأصل مع المجموعة الأولى وإضافة المجموعة باء إلى المجلد الفرعي الأول.</span><span class="sxs-lookup"><span data-stu-id="77d94-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="77d94-111">إيقاف مشاركة ملف أو مجلد</span><span class="sxs-lookup"><span data-stu-id="77d94-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

