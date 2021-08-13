---
title: تقييد الوصول في SharePoint أو OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: fc6731d5a7747bb4fc8d6cef1b6ac0045d11917d7f97abbb21eea9613b1b1aa2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54093758"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

هناك العديد من الطرق لتقييد الوصول إلى SharePoint عبر الإنترنت/OneDrive الخدمات. تم أدناه عرض طرق تقييد الوصول المختلفة هذه. 

**تقييد الأذونات**

في SharePoint عبر الإنترنت OneDrive for Business، نقوم بتقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات من خلال منح حق الوصول إلى تلك المجموعات/الأفراد الذين يجب أن يكون لديهم حق الوصول فقط.

- [تخصيص الأذونات لقائمة SharePoint أو مكتبة](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص SharePoint الموقع](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات في أحد ابر](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم في الوصول من الأجهزة غير المراقبة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

كمسؤول SharePoint عام، يمكنك حظر الوصول إلى محتوى SharePoint و OneDrive أو تقييده من الأجهزة غير الإدارة (تلك التي لم يتم ضمها إلى AD المختلط أو المتوافقة في Intune).

**تقييد موقع الشبكة**

بالاستناد إلى مواقع الشبكة المعرفة التي تثق بها، يمكنك التحكم في الوصول SharePoint الموارد OneDrive بها. يعرف ذلك أيضا باسم النهج المستند إلى الموقع. لمزيد من المعلومات، الرجاء الاطلاع على التحكم في الوصول إلى SharePoint عبر الإنترنت [OneDrive البيانات استنادا إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**تقييد تأمين الموقع** 

ضمن SharePoint Online لديك القدرة على تأمين مجموعة مواقع ويب، بحيث لا يمكن لأحد الوصول إليها. يتم تعيين هذا عبر PowerShell [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام [الخاصية Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState.

**تقييد المستخدمين من إنشاء المواقع أو المواقع الفرعية**

كمسؤول SharePoint أو مسؤول عام، يمكنك السماح للمستخدمين بإنشاء مواقع SharePoint الخاصة بهم وإدارتها، وتحديد نوع المواقع التي يمكنهم إنشاؤها، وتحديد موقع المواقع. لمزيد من المعلومات، الرجاء الاطلاع [على إدارة إنشاء الموقع في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

