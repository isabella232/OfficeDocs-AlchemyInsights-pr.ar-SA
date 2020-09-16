---
title: أزاله البيانات والاجهزه الويبينجه من Intune
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
ms.openlocfilehash: 24330dffb38be14dd369960ff86d4650d60c55ec
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47701270"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="d35dc-102">أزاله البيانات والاجهزه الويبينجه من Intune</span><span class="sxs-lookup"><span data-stu-id="d35dc-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="d35dc-103">يمكن استخدام الإجراءات البعيدة للغاء الجهاز ومسح الجهاز لأزاله بيانات الشركة المدارة بواسطة Intune أو لاجراء أعاده تعيين المصنع وإرجاع الجهاز إلى إعداداته الافتراضية.</span><span class="sxs-lookup"><span data-stu-id="d35dc-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="d35dc-104">سجل دخولك إلى أداره أجهزه Microsoft 365 ، وانتقل إلى **الاجهزه**  >  **كل الاجهزه**.</span><span class="sxs-lookup"><span data-stu-id="d35dc-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="d35dc-105">حدد الجهاز الذي تريد مسحه.</span><span class="sxs-lookup"><span data-stu-id="d35dc-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="d35dc-106">حدد نوع المسح البعيد الذي تريد القيام به.</span><span class="sxs-lookup"><span data-stu-id="d35dc-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="d35dc-107">قم بإيقاف حذف المعلومات التنظيمية فقط ، في حين مناديل الجهاز بالبالكامل إلى إعدادات المصنع.</span><span class="sxs-lookup"><span data-stu-id="d35dc-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="d35dc-108">حدد **نعم** للتاكيد.</span><span class="sxs-lookup"><span data-stu-id="d35dc-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="d35dc-109">حتى ينتهي المسح ، تظهر حاله اجراء الجهاز بالشكل المعلق.</span><span class="sxs-lookup"><span data-stu-id="d35dc-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="d35dc-110">بعد اكتمال الاجراء ، لن تتمكن من رؤية الجهاز المحمول في قائمه الاجهزه المدارة.</span><span class="sxs-lookup"><span data-stu-id="d35dc-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="d35dc-111">**ملاحظه** لا يمكن أزاله بيانات الشركة من الاجهزه المنضمة إلى Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d35dc-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="d35dc-112">للحصول علي التفاصيل الكاملة لتاثير الإيقاف والمسح ، بما في ذلك ما يتم الاحتفاظ به وحذفه ، راجع [أزاله الاجهزه باستخدام مسح أو إيقاف أو إلغاء الجهاز](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="d35dc-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="d35dc-113">لمسح كل البيانات من جهاز macOS ، راجع [محو كل البيانات من جهاز macOS](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="d35dc-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>