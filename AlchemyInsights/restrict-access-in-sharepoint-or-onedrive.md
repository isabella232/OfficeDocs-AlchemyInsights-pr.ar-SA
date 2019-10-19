---
title: تقييد الوصول في SharePoint أو اندريف
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551438"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="e68df-102">تقييد الوصول في SharePoint أو اندريف</span><span class="sxs-lookup"><span data-stu-id="e68df-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="e68df-103">في SharePoint و OneDrive ، يمكنك تقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم عن طريق منح حق الوصول فقط للمجموعات أو الافراد الذين تريد الوصول اليهم.</span><span class="sxs-lookup"><span data-stu-id="e68df-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="e68df-104">بشكل افتراضي ، يتم توريث الأذونات في SharePoint من اعلي في التسلسل الهرمي.</span><span class="sxs-lookup"><span data-stu-id="e68df-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="e68df-105">لذلك يرث ملف الأذونات الخاصة به من المجلد ، الذي يرث الأذونات الخاصة به من المكتبة ، التي ترث الأذونات الخاصة به من الموقع.</span><span class="sxs-lookup"><span data-stu-id="e68df-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="e68df-106">يمكنك المشاركة علي مستوي اعلي (مثلا عن طريق مشاركه موقع بأكمله) ثم قطع التوريث إذا كنت لا تريد مشاركه كافة العناصر الموجودة علي الموقع.</span><span class="sxs-lookup"><span data-stu-id="e68df-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="e68df-107">ومع ذلك ، لا ننصح بذلك لأنه يجعل الحفاظ علي الأذونات أكثر تعقيدا ومربكه في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="e68df-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="e68df-108">واليك ما يمكنك القيام به بدلا من ذلك:</span><span class="sxs-lookup"><span data-stu-id="e68df-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="e68df-109">إذا أردت ، علي سبيل المثال ، مشاركه كافة محتويات المجلد باستثناء ملف واحد فيه ، قم بنقل هذا الملف إلى موقع جديد غير مشترك.</span><span class="sxs-lookup"><span data-stu-id="e68df-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="e68df-110">إذا كان لديك اثنين من المجلدات الفرعية ، وتريد مشاركه مجلد فرعي واحد مع المجموعتين A و B والسماح فقط للمجموعة A بالوصول إلى المجلد الفرعي الثاني ، فقم بمشاركه المجلد الأصل مع المجموعة A وأضافه المجموعة B للمجلد الفرعي الأول.</span><span class="sxs-lookup"><span data-stu-id="e68df-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="e68df-111">إيقاف مشاركه ملف أو مجلد</span><span class="sxs-lookup"><span data-stu-id="e68df-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

