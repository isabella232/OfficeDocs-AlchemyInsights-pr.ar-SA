---
title: تقييد الوصول في SharePoint أو أندريف
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750651"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو أندريف

هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint على الإنترنت/أندريف. وترد أدناه أساليب تقييد الوصول المختلفة هذه. 

**تقييد الإذن**

في SharePoint Online وOneDrive for Business، نقوم بتقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات من خلال منح حق الوصول فقط إلى تلك المجموعات/الأفراد الذين يجب أن يكون لديهم حق الوصول.

- [تخصيص الأذونات لقائمة أو مكتبة SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص أذونات موقع SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات على مجلد فرعي](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم في الوصول من الأجهزة غير المُدارة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

كمسؤول SharePoint أو عمومي في Office 365، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint و OneDrive من الأجهزة غير المُدارة (تلك التي لم يتم ضمها AD المختلطأو متوافقة في إينتوني).

**تقييد موقع الشبكة**

بصفتك مسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint وOneDrive استنادًا إلى مواقع شبكة الاتصال المحددة التي تثق بها. يُعرف هذا أيضًا بالسياسة المستندة إلى الموقع. لمزيد من المعلومات، الرجاء [مراجعة التحكم في الوصول إلى بيانات SharePoint عبر الإنترنت وOneDrive استناداً إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**تقييد تأمين الموقع** 

داخل SharePoint على الإنترنت لديك القدرة على تأمين مجموعة موقع، لذلك لا أحد لديه حق الوصول. يتم تعيين هذا عبر PowerShell و [Shell إدارة SharePoint عبر الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام [الخاصية مجموعة SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) لوكستيت.

**تقييد المستخدمين من إنشاء مواقع أو مواقع فرعية**

بصفتك مسؤول SharePoint أو مسؤول عمومي Office 365، يمكنك السماح للمستخدمين بإنشاء وإدارة مواقع SharePoint الخاصة بهم، وتحديد نوع المواقع التي يمكنهم إنشاؤها، وتحديد موقع المواقع. لمزيد من المعلومات، الرجاء [مراجعة إدارة إنشاء الموقع في SharePoint على الإنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)

