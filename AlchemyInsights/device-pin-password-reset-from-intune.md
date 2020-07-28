---
title: إعادة تعيين دبوس/كلمة مرور الجهاز من Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1278"
- "6700008"
ms.openlocfilehash: fd3bb957b0da22dfab5a9988a82e398757e12ee5
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438706"
---
# <a name="device-pinpassword-reset-from-intune"></a><span data-ttu-id="d77b8-102">إعادة تعيين دبوس/كلمة مرور الجهاز من Intune</span><span class="sxs-lookup"><span data-stu-id="d77b8-102">Device pin/password reset from Intune</span></span>

<span data-ttu-id="d77b8-103">يمكنك إزالة رمز مرور أو إجبار مستخدم على إنشاء رمز مرور جديد في Intune لجهاز يعمل بنظام iOS أو Android باستخدام إجراء إزالة رمز المرور.</span><span class="sxs-lookup"><span data-stu-id="d77b8-103">You can remove a passcode or force a user to create a new passcode in Intune for a device running iOS or Android by using the Remove Passcode action.</span></span>

<span data-ttu-id="d77b8-104">تدعم أنواع نظام التشغيل وأنواع ملفات تعريف العمل هذا الإجراء فقط.</span><span class="sxs-lookup"><span data-stu-id="d77b8-104">Only specific operating system types and work profile types support this action.</span></span>

<span data-ttu-id="d77b8-105">للحصول على تفاصيل حول الأنظمة الأساسية المدعومة وكيفية تشغيل إجراء إعادة تعيين رمز المرور، راجع [إعادة تعيين رمز مرور الجهاز أو إزالته في Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span><span class="sxs-lookup"><span data-stu-id="d77b8-105">For details about supported platforms and how to trigger the reset passcode action, see [Reset or remove a device passcode in Intune](https://docs.microsoft.com/intune/device-passcode-reset).</span></span>

<span data-ttu-id="d77b8-106">يمكنك إعادة تعيين دبوس موجود إلى قيمة جديدة باستخدام إجراء "إعادة تعيين دبوس" على الأجهزة التي تعمل بنظام التشغيل Windows 10 المحمول.</span><span class="sxs-lookup"><span data-stu-id="d77b8-106">You can reset an existing pin to a new value using the Pin Reset action on devices running the Windows 10 Mobile operating system.</span></span> <span data-ttu-id="d77b8-107">هذا يسمح للمستخدم لفتح الجهاز وتعيين دبوس جديد حسب الاقتضاء.</span><span class="sxs-lookup"><span data-stu-id="d77b8-107">This allows the user to unlock the device and set a new pin as appropriate.</span></span> <span data-ttu-id="d77b8-108">لمزيد من المعلومات، راجع [إعادة تعيين رمز المرور على أجهزة Windows باستخدام Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span><span class="sxs-lookup"><span data-stu-id="d77b8-108">For more info, see [Reset the passcode on Windows devices using Intune](https://docs.microsoft.com/intune/device-windows-pin-reset).</span></span>