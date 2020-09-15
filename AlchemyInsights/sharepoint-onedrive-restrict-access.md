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
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700442"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>تقييد الوصول في SharePoint أو OneDrive

هناك العديد من الطرق لتقييد الوصول إلى خدمات SharePoint Online/OneDrive. يتم توضيح طرق تقييد الوصول المختلفة أدناه. 

**قيد الأذونات**

في SharePoint Online و OneDrive for Business ، قم بتقييد الوصول إلى عناصر مثل المواقع والملفات والمجلدات بمنح حق الوصول إلى هذه المجموعات/الأشخاص الذين يجب ان يملكون حق الوصول.

- [تخصيص الأذونات لقائمه أو مكتبه SharePoint](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [تخصيص أذونات موقع SharePoint](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [تغيير الأذونات علي مجلد فرعي](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [التحكم في الوصول من الاجهزه غير المدارة](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

بصفتك مسؤولا عموميا أو SharePoint ، يمكنك حظر الوصول إلى المحتوي SharePoint و OneDrive من الاجهزه غير المدارة أو تقييده (غير المرتبطة بالإعلانات المختلطة أو المتوافقة معها في Intune).

**تقييد موقع الشبكة**

بصفتك مسؤولا ، يمكنك التحكم في الوصول إلى موارد SharePoint و OneDrive استنادا إلى مواقع الشبكة المعرفة التي تثق بها. يعرف هذا أيضا باسم النهج المستند إلى الموقع. لمزيد من المعلومات ، يرجى مراجعه [التحكم في الوصول إلى بيانات SharePoint Online و OneDrive استنادا إلى موقع الشبكة](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

**قيد تامين الموقع** 

في SharePoint Online ، تتوفر لديك القدرة علي تامين مجموعه مواقع مشتركه ، لذلك لا يوجد لدي اي شخص حق الوصول. يتم تعيين ذلك عبر PowerShell و [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) باستخدام الخاصية [set سبوسيتي](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -لوكستاتي.

**منع المستخدمين من إنشاء مواقع أو مواقع فرعيه**

بصفتك مسؤول SharePoint أو مسؤول عمومي ، يمكنك السماح للمستخدمين بإنشاء مواقع SharePoint الخاصة بهم وأدارتها ، وتحديد نوع المواقع التي يمكنهم إنشاؤها ، وتحديد موقع المواقع. لمزيد من المعلومات ، يرجى مراجعه [إنشاء موقع الاداره في SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)

