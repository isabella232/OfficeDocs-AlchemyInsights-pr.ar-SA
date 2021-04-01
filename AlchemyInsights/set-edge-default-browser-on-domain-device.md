---
title: تعيين Microsoft Edge كمستعرض افتراضي على جهاز انضم إلى المجال
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491303"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="580c1-102">تعيين Microsoft Edge كمستعرض افتراضي على جهاز انضم إلى المجال</span><span class="sxs-lookup"><span data-stu-id="580c1-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="580c1-103">تعيين Microsoft Edge كمستعرض افتراضي:</span><span class="sxs-lookup"><span data-stu-id="580c1-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="580c1-104">[إنشاء ملف تكوين اقترانات افتراضي](https://go.microsoft.com/fwlink/?linkid=2132437) وتخزينه محليا أو على مشاركة شبكة.</span><span class="sxs-lookup"><span data-stu-id="580c1-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="580c1-105">افتح محرر نهج المجموعة، ثم انتقل إلى **قوالب تكوين** الكمبيوتر الإدارية في مستكشف الملفات  >    >  **لمكونات Windows**  >  .</span><span class="sxs-lookup"><span data-stu-id="580c1-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="580c1-106">حدد **تعيين ملف تكوين اقترانات افتراضي**.</span><span class="sxs-lookup"><span data-stu-id="580c1-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="580c1-107">حدد **إعداد النهج**، ثم حدد **تمكين**.</span><span class="sxs-lookup"><span data-stu-id="580c1-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="580c1-108">ضمن **خيارات**، أدخل موقع ملف تكوين الاقترانات الافتراضي، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="580c1-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
