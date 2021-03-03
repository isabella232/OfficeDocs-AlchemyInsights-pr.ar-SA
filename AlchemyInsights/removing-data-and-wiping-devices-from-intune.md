---
title: إزالة البيانات ومسح الأجهزة من Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416300"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="ac749-102">إزالة البيانات ومسح الأجهزة من Intune</span><span class="sxs-lookup"><span data-stu-id="ac749-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="ac749-103">يمكن استخدام الإجراءين "إيقاف الجهاز" و"مسح الجهاز" عن بعد لإزالة بيانات الشركة المدارة بواسطة Intune أو لتنفيذ عملية إعادة ضبط المصنع وإعادة الجهاز إلى إعداداته الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="ac749-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="ac749-104">سجل الدخول إلى Microsoft 365 Device Management، واذهب إلى **"الأجهزة**  >  **كافة الأجهزة".**</span><span class="sxs-lookup"><span data-stu-id="ac749-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="ac749-105">حدد الجهاز الذي تريد مسحه.</span><span class="sxs-lookup"><span data-stu-id="ac749-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="ac749-106">حدد نوع المسح عن بعد الذي تريد القيام به.</span><span class="sxs-lookup"><span data-stu-id="ac749-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="ac749-107">يحذف إيقاف المعلومات التنظيمية فقط، بينما تستعيد عمليات المسح الكامل الجهاز إلى إعدادات المصنع الخاصة به.</span><span class="sxs-lookup"><span data-stu-id="ac749-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="ac749-108">حدد **"نعم"** لتأكيد الأمر.</span><span class="sxs-lookup"><span data-stu-id="ac749-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="ac749-109">حتى تنتهي عملية المسح، تظهر حالة الإجراء "الجهاز" ك *"معلق للتقاعد".*</span><span class="sxs-lookup"><span data-stu-id="ac749-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="ac749-110">بعد اكتمال الإجراء، لن ترى الجهاز المحمول بعد الآن في قائمة الجهاز المدار.</span><span class="sxs-lookup"><span data-stu-id="ac749-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="ac749-111">لا يمكن إزالة بيانات الشركة من الأجهزة المنضمة إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ac749-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="ac749-112">للحصول على التفاصيل الكاملة حول تأثير إجراءات "إيقاف" و"مسح"، بما في ذلك ما تم الاحتفاظ به وما تم حذفه، راجع الوثائق التالية:</span><span class="sxs-lookup"><span data-stu-id="ac749-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="ac749-113">[قم بإزالة الأجهزة باستخدام مسح](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe)الجهاز أو إيقافه أو إلغاءه يدويا.</span><span class="sxs-lookup"><span data-stu-id="ac749-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="ac749-114">كيفية مسح بيانات الشركة فقط من تطبيقات Intune المدارة</span><span class="sxs-lookup"><span data-stu-id="ac749-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="ac749-115">[مسح كل البيانات من جهاز macOS.](https://docs.microsoft.com/mem/intune/remote-actions/device-erase)</span><span class="sxs-lookup"><span data-stu-id="ac749-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>