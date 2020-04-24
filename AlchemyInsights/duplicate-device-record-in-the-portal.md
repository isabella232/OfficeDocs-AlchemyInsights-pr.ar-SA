---
title: سجل جهاز مكرر في المدخل
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9001495"
- "4386"
ms.openlocfilehash: 277afc59705e6040f0f9ae0c8cad965bd7d3ef65
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789515"
---
# <a name="duplicate-device-record-in-the-portal"></a><span data-ttu-id="9edaa-102">سجل جهاز مكرر في المدخل</span><span class="sxs-lookup"><span data-stu-id="9edaa-102">Duplicate device record in the portal</span></span>

<span data-ttu-id="9edaa-103">يمكنك رؤية سجلين للجهاز في المدخل، إذا لم يقم الجهاز بالإبلاغ عن حالة الإدارة المشتركة بشكل صحيح في موقع إدارة التكوين.</span><span class="sxs-lookup"><span data-stu-id="9edaa-103">You may see 2 records for a device in the portal if the device does not correctly report the co-management status to the Configuration Manager site.</span></span> <span data-ttu-id="9edaa-104">للتحقق من حالة الإدارة المشتركة للجهاز، راجع عمود **الإدارة المشتركة** للجهاز في وحدة تحكم إدارة التكوين.</span><span class="sxs-lookup"><span data-stu-id="9edaa-104">To check the co-management status of a device, review the **Co-managed** column for the device in the Configuration Manager console.</span></span> <span data-ttu-id="9edaa-105">إذا لم يكن العمود مرئياً، فيمكنك إضافته بالنقر بزر الماوس الأيمن فوق أي من رؤوس الأعمدة، وتحديده من القائمة.</span><span class="sxs-lookup"><span data-stu-id="9edaa-105">If the column is not visible, you may add it by right-clicking any of the column headers, and selecting it from the list.</span></span>

<span data-ttu-id="9edaa-106">القيمة المُدارة بشكل مشترك يجب أن تكون **نعم**.</span><span class="sxs-lookup"><span data-stu-id="9edaa-106">The Co-managed value must be **Yes**.</span></span> <span data-ttu-id="9edaa-107">إذا كانت القيمة هي **لا**، فافتح التطبيق الصغير لعميل إدارة التكوين على جهاز العميل وتحقق من خاصية **الإدارة المشتركة** في علامة التبويب "عام".</span><span class="sxs-lookup"><span data-stu-id="9edaa-107">If the value is **No**, open the Configuration Manager client applet on the client device and check the **Co-management** property in the General tab.</span></span>

- <span data-ttu-id="9edaa-108">إذا كانت القيمة هي **ممكَّن**، فهذا يشير إلى وجود مشاكل تتعلق باتصال العميل مع نقطة الإدارة.</span><span class="sxs-lookup"><span data-stu-id="9edaa-108">If the value is **Enabled**, this indicates problems with client communication with the Management Point.</span></span> <span data-ttu-id="9edaa-109">رجاءً راجع **CcmMessaging.log** على الجهاز للتحقق من مشاكل الاتصال المحتملة.</span><span class="sxs-lookup"><span data-stu-id="9edaa-109">Please review the **CcmMessaging.log** on the device to investigate potential connectivity issues.</span></span>

- <span data-ttu-id="9edaa-110">إذا كانت القيمة هي **معطّل** وتم تسجيل الجهاز في Intune، فرجاءً تأكد من أن الجهاز قد تلقى نهج الإدارة المشتركة من خلال مراجعة **CoManagementHandler.log** على الجهاز.</span><span class="sxs-lookup"><span data-stu-id="9edaa-110">If the value is **Disabled** and the device is enrolled in Intune, please ensure that the device has received the Co-management policy by reviewing the **CoManagementHandler.log** on the device.</span></span>
