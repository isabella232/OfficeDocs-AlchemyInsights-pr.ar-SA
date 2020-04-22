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
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

في SharePoint و OneDrive، تقوم بتقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم عن طريق منح حق الوصول فقط إلى المجموعات أو الأفراد الذين تريد الوصول إليها. بشكل افتراضي، يتم توريث الأذونات في SharePoint من أعلى في التسلسل الهرمي. لذلك يرث ملف أذوناته من المجلد الذي يرث أذوناته من المكتبة التي ترث أذوناتها من الموقع.
  
يمكنك المشاركة على مستوى أعلى (مثل مشاركة موقع بأكمله) ثم قطع الوراثة إذا كنت لا تريد مشاركة جميع العناصر على الموقع. ومع ذلك، لا نوصي بذلك لأنه يجعل الحفاظ على الأذونات أكثر تعقيدًا وإرباكًا في المستقبل. إليك ما يمكنك القيام به بدلاً من ذلك:
  
- على سبيل المثال، إذا كنت تريد مشاركة كافة محتويات مجلد باستثناء ملف واحد فيه، فانتقل هذا الملف إلى موقع جديد غير مشترك.
    
- إذا كان لديك مجلدين فرعيين في مجلد، وتريد مشاركة مجلد فرعي واحد مع المجموعتين A و B والسماح فقط للمجموعة A بالوصول إلى المجلد الفرعي الثاني، فشارك المجلد الأصل مع المجموعة A وأضف المجموعة B إلى المجلد الفرعي الأول.
    
[إيقاف مشاركة ملف أو مجلد](https://go.microsoft.com/fwlink/?linkid=2008861)
  

