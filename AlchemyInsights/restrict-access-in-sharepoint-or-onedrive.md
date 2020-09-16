---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720669"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="c0fbb-102">تقييد الوصول في SharePoint أو OneDrive</span><span class="sxs-lookup"><span data-stu-id="c0fbb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="c0fbb-103">في SharePoint و OneDrive ، يمكنك تقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم عن طريق منح حق الوصول إلى المجموعات أو الأشخاص الذين تريدهم ان يتوفر لديهم الاذن.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="c0fbb-104">بشكل افتراضي ، يتم توريث الأذونات في SharePoint من المستوي الأعلى في التسلسل الهيكلي.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="c0fbb-105">لذلك يرث الملف الأذونات الخاصة به من المجلد ، الذي يرث الأذونات الخاصة به من المكتبة ، التي ترث الأذونات الخاصة به من الموقع.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="c0fbb-106">يمكنك المشاركة علي مستوي اعلي (مثل مشاركه موقع بأكمله) ثم قطع التوريث إذا لم تكن ترغب في مشاركه كل العناصر الموجودة علي الموقع.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="c0fbb-107">علي الرغم من ذلك ، لا نوصي بهذا الاجراء لأنه يجعل الأذونات أكثر تعقيدا ومربكا في المستقبل.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="c0fbb-108">اليك ما يمكنك فعله بدلا من ذلك:</span><span class="sxs-lookup"><span data-stu-id="c0fbb-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="c0fbb-109">علي سبيل المثال ، إذا كنت تريد مشاركه كل محتويات المجلد باستثناء ملف واحد ، فانقل هذا الملف إلى موقع جديد غير مشترك.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="c0fbb-110">إذا كان لديك مجلدين فرعيين في الملف ، وكانت تريد مشاركه مجلد فرعي واحد مع المجموعتين A و B والسماح فقط بالوصول إلى المجلد الفرعي الثاني ، فيمكنك مشاركه المجلد الأصل مع المجموعة ا وأضافه المجموعة ب إلى المجلد الفرعي الأول.</span><span class="sxs-lookup"><span data-stu-id="c0fbb-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="c0fbb-111">إيقاف مشاركه ملف أو مجلد </span><span class="sxs-lookup"><span data-stu-id="c0fbb-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

