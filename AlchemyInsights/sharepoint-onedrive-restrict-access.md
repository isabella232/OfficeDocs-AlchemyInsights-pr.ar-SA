---
title: تقييد الوصول في SharePoint أو أندريف
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559864"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو أندريف

هناك العديد من الطرق لتقييد الوصول إلى خدمات عبر الإنترنت/أندريف SharePoint. يلي هذه الطرق تقييد وصول مختلف. 

**تقييد الإذن**

في SharePoint على الإنترنت وأونيدريفي للعمل، نحن تقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات بمنح حق الوصول إلى المجموعات/الأفراد الذين ينبغي أن تتاح فقط.

- [تخصيص الأذونات لمكتبة أو قائمة SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص أذونات موقع SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات على مجلد فرعي](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم بالوصول من الأجهزة غير المدارة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

ك SharePoint أو المسؤول العمومي في Office 365، يمكنك حظر أو تقييد الوصول إلى محتوى SharePoint وأندريف من الأجهزة غير المدارة (تلك المختلط الإعلانية المرتبطة أو متوافقة في إينتوني).

**قيود موقع الشبكة**

كمسؤول تكنولوجيا المعلومات، يمكنك التحكم في الوصول إلى موارد SharePoint وأندريف استناداً إلى شبكة المعرفة المواقع الموثوق بها. هذا يعرف أيضا نهج يستند إلى الموقع. لمزيد من المعلومات، انظر [التحكم في الوصول إلى SharePoint والبيانات أندريف استناداً إلى موقع شبكة الاتصال](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**قيد تأمين الموقع** 

في SharePoint على الإنترنت لديك القدرة على تأمين مجموعة موقع، حيث لا أحد يملك حق الوصول. يتم تعيين هذه عبر PowerShell واستخدام الخاصية-LockState [سبوسيتي مجموعة](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) [SharePoint Shell إدارة الإنترنت](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) .

**منع المستخدمين من إنشاء المواقع أو المواقع الفرعية**

كمسؤول SharePoint أو المسؤول العمومي Office 365، يمكنك السماح للمستخدمين بإنشاء وإدارة مواقع SharePoint الخاصة بهم، وتحديد أي نوع من المواقع التي يمكن أن تخلق، ثم عين الموقع المواقع. لمزيد من المعلومات، انظر [إنشاء موقع إدارة في SharePoint عبر إنترنت](https://docs.microsoft.com/sharepoint/manage-site-creation)

