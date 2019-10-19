---
title: تقييد الوصول في SharePoint أو اندريف
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36750651"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو اندريف

هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint علي الإنترنت/اندريف. هذه الطرق المختلفة لتقييد الوصول موضحه أدناه. 

**تقييد الأذونات**

في SharePoint علي الإنترنت و اندريف للعمل ، ونحن تقييد الوصول إلى العناصر مثل المواقع والملفات والمجلدات عن طريق منح حق الوصول إلى تلك المجموعات/الافراد الذين يجب ان يكون الوصول.

- [تخصيص أذونات لقائمه أو مكتبه SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص أذونات موقع SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات علي مجلد فرعي](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم في الوصول من الاجهزه غير المدارة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

كمسؤول SharePoint أو العمومية في Office 365 ، يمكنك حظر أو تقييد الوصول إلى محتوي SharePoint و OneDrive من الاجهزه غير المدارة (تلك غير المختلطة AD منضمة أو متوافقة في اينتوني).

**تقييد موقع الشبكة**

بصفتك مسؤول تكنولوجيا الاتصال ، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادا إلى مواقع الشبكة المعرفة التي تثق بها. ويعرف هذا أيضا باسم النهج المستند إلى الموقع. لمزيد من المعلومات ، الرجاء مراجعه [التحكم بالوصول إلى SharePoint علي الإنترنت والبيانات اندريف استنادا إلى موقع شبكه الاتصال](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**تقييد قفل الموقع** 

داخل SharePoint علي الإنترنت لديك القدرة علي تامين مجموعه موقع ، لذلك لا أحد لديه حق الوصول. يتم تعيين هذا عبر PowerShell و [Shell أداره SharePoint علي الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام الخاصية [مجموعه sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.

**تقييد المستخدمين من إنشاء مواقع أو مواقعه فرعيه**

كمسؤول SharePoint أو المسؤول العمومي Office 365 ، يمكنك السماح للمستخدمين إنشاء وأداره مواقع SharePoint الخاصة بهم ، وتحديد اي نوع من المواقع التي يمكن إنشاؤها ، وتحديد موقع المواقع. لمزيد من المعلومات ، الرجاء مراجعه [أداره إنشاء الموقع في SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)

