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
ms.openlocfilehash: b7b68df2ae24b09fe9b01bd67c31a89e37f284a512bc1ecb097ef52fae5ae7d6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54075027"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

في SharePoint OneDrive، يمكنك تقييد الوصول إلى عناصر مثل الملفات والمجلدات والقوائم من خلال منح حق الوصول إلى المجموعات أو الأفراد الذين تريد الوصول إليها فقط. بشكل افتراضي، يتم توارث SharePoint من أعلى إلى أعلى في التسلسل الهيكلي. وبالتالي، يرث الملف أذوناته من المجلد، الذي يرث أذوناته من المكتبة، التي ترث أذوناته من الموقع.
  
يمكنك المشاركة على مستوى أعلى (مثل مشاركة موقع بأكمله) ثم قطع التوريث إذا كنت لا تريد مشاركة كل العناصر على الموقع. ومع ذلك، لا نوصي بذلك لأنه يجعل الاحتفاظ بالأذونات أكثر تعقيدا ومربكا في المستقبل. إليك ما يمكنك فعله بدلا من ذلك:
  
- إذا أردت، على سبيل المثال، مشاركة كل محتويات مجلد ما باستثناء ملف واحد فيه، فحرك هذا الملف إلى موقع جديد غير مشترك.
    
- إذا كان لديك مجلدان فرعيون في مجلد، وتريد مشاركة مجلد فرعي واحد مع المجموعتين A وB والسماح فقط للمجموعة A بالوصول إلى المجلد الفرعي الثاني، فشارك المجلد الأصل مع المجموعة A وأضف المجموعة B إلى المجلد الفرعي الأول.
    
[إيقاف مشاركة ملف أو مجلد ](https://go.microsoft.com/fwlink/?linkid=2008861)
  

