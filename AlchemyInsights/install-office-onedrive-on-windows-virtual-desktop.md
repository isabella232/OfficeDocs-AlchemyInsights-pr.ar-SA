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
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="8c943-102">تثبيت Office و OneDrive على سطح المكتب الافتراضي ل Windows</span><span class="sxs-lookup"><span data-stu-id="8c943-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="8c943-103">[قم بإعداد صورة VHD رئيسية وتخصيصها](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span><span class="sxs-lookup"><span data-stu-id="8c943-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="8c943-104">قم بإنشاء جهاز ظاهري (VM) إذا لم يتم إنشاؤه بالفعل.</span><span class="sxs-lookup"><span data-stu-id="8c943-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="8c943-105">[تثبيت Office في وضع تنشيط الكمبيوتر المشترك](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span><span class="sxs-lookup"><span data-stu-id="8c943-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="8c943-106">يتيح التنشيط المشترك للكمبيوتر لعدة مستخدمين الوصول إلى Office.</span><span class="sxs-lookup"><span data-stu-id="8c943-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="8c943-107">[تثبيت OneDrive في الوضع لكل جهاز.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="8c943-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="8c943-108">عادة، يتم تثبيت OneDrive لكل مستخدم، ولكن هنا، يجب تثبيته لكل جهاز.</span><span class="sxs-lookup"><span data-stu-id="8c943-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>