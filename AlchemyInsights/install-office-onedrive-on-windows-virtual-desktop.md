---
title: تثبيت Office OneDrive على Windows سطح المكتب الظاهري
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 226bd24a955f6165969102c8cf00cf45da537ee05a5363c74f1dfd055d922e1d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028603"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>تثبيت Office OneDrive على Windows سطح المكتب الظاهري

1. [قم بإعداد صورة VHD رئيسية وتخصيصها](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). قم بإنشاء جهاز ظاهري (VM) إذا لم يتم إنشاؤه بالفعل.

1. [تثبيت Office في وضع تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). يتيح التنشيط المشترك للكمبيوتر لعدة مستخدمين الوصول إلى Office.

1. [تثبيت OneDrive في وضع كل جهاز.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) عادة، OneDrive يتم تثبيتها لكل مستخدم، ولكن هنا، يجب تثبيتها لكل جهاز.