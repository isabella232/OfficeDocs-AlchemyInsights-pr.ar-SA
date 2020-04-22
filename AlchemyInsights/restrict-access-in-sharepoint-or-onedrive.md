---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715871"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="510c1-102">تقييد الوصول في SharePoint أو OneDrive</span><span class="sxs-lookup"><span data-stu-id="510c1-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="510c1-103">في SharePoint و OneDrive، تقوم بتقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم عن طريق منح حق الوصول فقط إلى المجموعات أو الأفراد الذين تريد الوصول إليها.</span><span class="sxs-lookup"><span data-stu-id="510c1-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="510c1-104">بشكل افتراضي، يتم توريث الأذونات في SharePoint من أعلى في التسلسل الهرمي.</span><span class="sxs-lookup"><span data-stu-id="510c1-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="510c1-105">لذلك يرث ملف أذوناته من المجلد الذي يرث أذوناته من المكتبة التي ترث أذوناتها من الموقع.</span><span class="sxs-lookup"><span data-stu-id="510c1-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="510c1-106">يمكنك المشاركة على مستوى أعلى (مثل مشاركة موقع بأكمله) ثم قطع الوراثة إذا كنت لا تريد مشاركة جميع العناصر على الموقع.</span><span class="sxs-lookup"><span data-stu-id="510c1-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="510c1-107">ومع ذلك، لا نوصي بذلك لأنه يجعل الحفاظ على الأذونات أكثر تعقيدًا وإرباكًا في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="510c1-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="510c1-108">إليك ما يمكنك القيام به بدلاً من ذلك:</span><span class="sxs-lookup"><span data-stu-id="510c1-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="510c1-109">على سبيل المثال، إذا كنت تريد مشاركة كافة محتويات مجلد باستثناء ملف واحد فيه، فانتقل هذا الملف إلى موقع جديد غير مشترك.</span><span class="sxs-lookup"><span data-stu-id="510c1-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="510c1-110">إذا كان لديك مجلدين فرعيين في مجلد، وتريد مشاركة مجلد فرعي واحد مع المجموعتين A و B والسماح فقط للمجموعة A بالوصول إلى المجلد الفرعي الثاني، فشارك المجلد الأصل مع المجموعة A وأضف المجموعة B إلى المجلد الفرعي الأول.</span><span class="sxs-lookup"><span data-stu-id="510c1-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="510c1-111">إيقاف مشاركة ملف أو مجلد</span><span class="sxs-lookup"><span data-stu-id="510c1-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

