---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 39aa8cd6e649eca4a1e196eeb589a825364d0977
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43692752"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint Online/OneDrive. وفيما يلي طرق تقييد الوصول المختلفة هذه. 

**تقييد الإذن**

في SharePoint Online و OneDrive للأعمال، نقيد الوصول إلى عناصر مثل المواقع والملفات والمجلدات من خلال منح حق الوصول فقط إلى تلك المجموعات /الأفراد الذين يجب أن يكون لديهم حق الوصول.

- [تخصيص أذونات لقائمة SharePoint أو مكتبة](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص أذونات موقع SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات على مجلد فرعي](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم في الوصول من الأجهزة غير المدارة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

كـ SharePoint أو مسؤول عمومي، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint وOneDrive من الأجهزة غير المدارة (تلك التي لا ينضم إليها الإعلان المختلط أو متوافقمعها في Intune).

**تقييد موقع الشبكة**

كمسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادًا إلى مواقع الشبكة المحددة التي تثق بها. ويُعرف هذا أيضًا باسم النهج المستند إلى الموقع. لمزيد من المعلومات، يرجى الاطلاع [على التحكم في الوصول إلى بيانات SharePoint Online و OneDrive استنادًا إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**تقييد قفل الموقع** 

داخل SharePoint Online لديك القدرة على تأمين مجموعة مواقع ، لذلك لا أحد لديه حق الوصول. يتم تعيين هذا عبر PowerShell [وSharePoint إدارة الإنترنت شل](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام [خاصية Set-SPOSite-LockState.](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps)

**تقييد المستخدمين من إنشاء مواقع أو مواقع فرعية**

كمسؤول SharePoint أو مسؤول عالمي، يمكنك السماح للمستخدمين بإنشاء مواقع SharePoint الخاصة بهم وإدارتها، وتحديد نوع المواقع التي يمكنهم إنشاؤها، وتحديد موقع المواقع. لمزيد من المعلومات، يرجى [الاطلاع على إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

