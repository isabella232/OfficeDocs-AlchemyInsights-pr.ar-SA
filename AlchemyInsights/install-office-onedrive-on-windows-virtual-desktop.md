---
title: تثبيت Office و OneDrive على سطح المكتب الافتراضي ل Windows
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
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595423"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>تثبيت Office و OneDrive على سطح المكتب الافتراضي ل Windows

1. [قم بإعداد صورة VHD رئيسية وتخصيصها](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image). قم بإنشاء جهاز ظاهري (VM) إذا لم يتم إنشاؤه بالفعل.

1. [تثبيت Office في وضع تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode). يتيح التنشيط المشترك للكمبيوتر لعدة مستخدمين الوصول إلى Office.

1. [تثبيت OneDrive في الوضع لكل جهاز.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode) عادة، يتم تثبيت OneDrive لكل مستخدم، ولكن هنا، يجب تثبيته لكل جهاز.