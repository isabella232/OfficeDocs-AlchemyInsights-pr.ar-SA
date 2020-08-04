---
title: استخدام ملفات تعريف البريد الإلكتروني مع Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "46554713"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="2c3b6-102">استخدام ملفات تعريف البريد الإلكتروني مع Intune</span><span class="sxs-lookup"><span data-stu-id="2c3b6-102">Using email profiles with Intune</span></span>

<span data-ttu-id="2c3b6-103">يمكن استخدام Intune لإنشاء ملفات تعريف البريد الإلكتروني ونشرها لعميل البريد الإلكتروني الأصلي (المدمج) على أنظمة أساسية متعددة للأجهزة.</span><span class="sxs-lookup"><span data-stu-id="2c3b6-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="2c3b6-104">للحصول على معلومات حول بعض القيود المرتبطة بملفات تعريف البريد الإلكتروني، بما في ذلك كيفية التعامل مع وجود ملفات التعريف الموجودة وكيفية إزالة ملفات تعريف البريد الإلكتروني، راجع [إضافة إعدادات البريد الإلكتروني إلى الأجهزة باستخدام Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="2c3b6-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="2c3b6-105">لمزيد من المعلومات حول كيفية إنشاء ملفات تعريف البريد الإلكتروني لكل نظام أساسي للجهاز، راجع:</span><span class="sxs-lookup"><span data-stu-id="2c3b6-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="2c3b6-106">إعدادات جهاز Android لتكوين البريد الإلكتروني والمصادقة والمزامنة في Intune</span><span class="sxs-lookup"><span data-stu-id="2c3b6-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="2c3b6-107">إضافة إعدادات البريد الإلكتروني لأجهزة iOS و iPadOS في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2c3b6-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="2c3b6-108">إعدادات ملف تعريف البريد الإلكتروني في Microsoft Intune للأجهزة التي تعمل بنظام Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="2c3b6-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="2c3b6-109">إعدادات ملف تعريف البريد الإلكتروني للأجهزة التي تعمل بنظام التشغيل Windows 10 في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="2c3b6-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="2c3b6-110">**مشكلة مزامنة شائعة**</span><span class="sxs-lookup"><span data-stu-id="2c3b6-110">**Common syncing issue**</span></span>

<span data-ttu-id="2c3b6-111">**يمنع ملف تعريف KNOX على البريد الإلكتروني Android جهات اتصال المستخدم والتقويم والمهام من المزامنة مع أجهزة المستخدم.**</span><span class="sxs-lookup"><span data-stu-id="2c3b6-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="2c3b6-112">يقدم ملف تعريف البريد الإلكتروني لـ KNOX على Android KNOX للمشرف خيار تحديد أنواع المحتوى التي تتم مزامنةها مع الجهاز عن طريق إعداد كل منها على تمكين.</span><span class="sxs-lookup"><span data-stu-id="2c3b6-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="2c3b6-113">إذا تم تعيين الإعداد لأي من أنواع المحتوى إلى **غير مكوّن** (الافتراضي)، فإن نوع المحتوى هذا غير متزامن تلقائياً.</span><span class="sxs-lookup"><span data-stu-id="2c3b6-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="2c3b6-114">قد يقوم المستخدم بتمكين نوع المحتوى الذي يريده مباشرةً على الجهاز يدوياً، ولكن يتم الكتابة فوق هذا التكوين بواسطة إعداد نهج Intune، وتتوقف المزامنة لنوع المحتوى هذا.</span><span class="sxs-lookup"><span data-stu-id="2c3b6-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

