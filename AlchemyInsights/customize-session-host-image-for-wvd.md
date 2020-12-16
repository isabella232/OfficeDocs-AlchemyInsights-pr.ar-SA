---
title: تخصيص صوره مضيف جلسة العمل لسطح مكتب Windows الظاهري
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003902"
- "6957"
ms.openlocfilehash: 23bf130aad5bafa6756f0adfc2e58a130c2f6c4e
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49691917"
---
# <a name="customize-a-session-host-image-for-windows-virtual-desktop"></a><span data-ttu-id="c84ac-102">تخصيص صوره مضيف جلسة العمل لسطح مكتب Windows الظاهري</span><span class="sxs-lookup"><span data-stu-id="c84ac-102">Customize a session host image for Windows Virtual Desktop</span></span>

<span data-ttu-id="c84ac-103">هناك طريقتان لتحضير جهاز ظاهري (VM) باستخدام صوره القرص الثابت الرئيسي الأساسي لنظام التشغيل Windows الظاهري:</span><span class="sxs-lookup"><span data-stu-id="c84ac-103">There are two ways to prepare a virtual machine (VM) by using a master Virtual Hard Disk image for Windows Virtual Desktop:</span></span>

1. <span data-ttu-id="c84ac-104">[قم بإنشاء VM من صوره مداره في Azure](https://go.microsoft.com/fwlink/?linkid=2127906)، ثم انتقل إلى الامام [لاعداد البرنامج وتثبيته](https://go.microsoft.com/fwlink/?linkid=2128064).</span><span class="sxs-lookup"><span data-stu-id="c84ac-104">[Create a VM from a managed image in Azure](https://go.microsoft.com/fwlink/?linkid=2127906), and then skip ahead to the [preparation and installation of software](https://go.microsoft.com/fwlink/?linkid=2128064).</span></span>
1. <span data-ttu-id="c84ac-105">[قم بإنشاء الصورة محليا](https://go.microsoft.com/fwlink/?linkid=2128065) بتنزيل الصورة وتوفير ملفات الوصول إلى الإصدار الواحد من نوع الملف [التشعبي](https://go.microsoft.com/fwlink/?linkid=2127907)بتنسيق VM ، ثم تخصيصها بما يتناسب مع احتياجاتك.</span><span class="sxs-lookup"><span data-stu-id="c84ac-105">[Create the image locally](https://go.microsoft.com/fwlink/?linkid=2128065) by downloading the image, [provisioning a Hyper-V VM](https://go.microsoft.com/fwlink/?linkid=2127907), and then customizing it to suit your needs.</span></span>

<span data-ttu-id="c84ac-106">لمعرفه المزيد ، راجع [تحضير صوره VHD الرئيسية وتخصيصها](https://go.microsoft.com/fwlink/?linkid=2127838).</span><span class="sxs-lookup"><span data-stu-id="c84ac-106">To learn more, see [Prepare and customize a master VHD image](https://go.microsoft.com/fwlink/?linkid=2127838).</span></span>