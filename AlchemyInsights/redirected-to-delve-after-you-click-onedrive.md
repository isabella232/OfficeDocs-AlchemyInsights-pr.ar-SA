---
title: OneDrive for Business Web OneDrive يعيد التوجيه إلى Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799976"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>تمت إعادة التوجيه إلى Delve بعد النقر فوق OneDrive

راجع دليل [استكشاف الأخطاء وإصلاحها التفصيلي.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

لحل هذه المشكلة، يجب على المسؤول منح المستخدمين الحق في إنشاء موقع "المواقع الخاصة بهم". وذلك لأن صفحة OneDrive for Business تم إنشاؤها على "المواقع الخاصة".

لمنح هذا الحق، اتبع الخطوات التالية:

1. في مركز إدارة SharePoint، انقر فوق **ملفات تعريف المستخدمين**.

2. في المقطع **الأشخاص،** انقر فوق **إدارة أذونات المستخدم**.

3. أضف المستخدمين الذين يحتاجون إلى أذونات لإنشاء موقع المواقع الخاصة بهم. بشكل افتراضي، يتم تعيين هذا الإعداد إلى **الجميع باستثناء المستخدمين الخارجيين**.

4. بعد إضافة المستخدم أو المستخدمين أو المجموعة، تأكد من تحديد المستخدم أو المستخدمين أو  المجموعة المضافة، قم بالتمرير إلى مقطع الأذونات، ثم حدد خانة الاختيار بجانب إنشاء موقع شخصي (مطلوب للتخزين الشخصي وملف الأخبار والمحتوى الذي **يليه).**

5. انقر **فوق** موافق ، ثم اسمح للمستخدم بالاستعراض إلى صفحة OneDrive لإنشاء الموقع.
