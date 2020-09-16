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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

في SharePoint و OneDrive ، يمكنك تقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم عن طريق منح حق الوصول إلى المجموعات أو الأشخاص الذين تريدهم ان يتوفر لديهم الاذن. بشكل افتراضي ، يتم توريث الأذونات في SharePoint من المستوي الأعلى في التسلسل الهيكلي. لذلك يرث الملف الأذونات الخاصة به من المجلد ، الذي يرث الأذونات الخاصة به من المكتبة ، التي ترث الأذونات الخاصة به من الموقع.
  
يمكنك المشاركة علي مستوي اعلي (مثل مشاركه موقع بأكمله) ثم قطع التوريث إذا لم تكن ترغب في مشاركه كل العناصر الموجودة علي الموقع. علي الرغم من ذلك ، لا نوصي بهذا الاجراء لأنه يجعل الأذونات أكثر تعقيدا ومربكا في المستقبل. اليك ما يمكنك فعله بدلا من ذلك:
  
- علي سبيل المثال ، إذا كنت تريد مشاركه كل محتويات المجلد باستثناء ملف واحد ، فانقل هذا الملف إلى موقع جديد غير مشترك.
    
- إذا كان لديك مجلدين فرعيين في الملف ، وكانت تريد مشاركه مجلد فرعي واحد مع المجموعتين A و B والسماح فقط بالوصول إلى المجلد الفرعي الثاني ، فيمكنك مشاركه المجلد الأصل مع المجموعة ا وأضافه المجموعة ب إلى المجلد الفرعي الأول.
    
[إيقاف مشاركه ملف أو مجلد ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

