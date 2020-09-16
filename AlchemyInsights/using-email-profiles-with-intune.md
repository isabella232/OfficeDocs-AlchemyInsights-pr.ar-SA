---
title: استخدام ملفات تعريف البريد الكتروني مع Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 92d91de5d369eb9d0ffde2580b75376035a6945b
ms.sourcegitcommit: 483444ab35ab0e4d410d121562045efde47aa61a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47653275"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="68fc0-102">استخدام ملفات تعريف البريد الكتروني مع Intune</span><span class="sxs-lookup"><span data-stu-id="68fc0-102">Using email profiles with Intune</span></span>

<span data-ttu-id="68fc0-103">يمكن استخدام Intune لإنشاء ملفات تعريف البريد الكتروني ونشرها لعميل البريد الكتروني الأصلي (المضمن) علي الانظمه الاساسيه للاجهزه المتعددة.</span><span class="sxs-lookup"><span data-stu-id="68fc0-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="68fc0-104">للحصول علي معلومات حول بعض القيود المقترنة بملفات تعريف البريد الكتروني ، بما في ذلك الطريقة التي تتم بها معالجه ملفات التعريف الموجودة وكيفيه أزاله ملفات تعريف البريد الكتروني ، راجع [أضافه إعدادات البريد الكتروني إلى الاجهزه التي تستخدم Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="68fc0-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="68fc0-105">للحصول علي مزيد من المعلومات حول كيفيه إنشاء ملفات تعريف البريد الكتروني لكل نظام أساسي للجهاز ، راجع:</span><span class="sxs-lookup"><span data-stu-id="68fc0-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="68fc0-106">إعدادات جهاز Android لتكوين البريد الكتروني والمصادقة والمزامنة في Intune</span><span class="sxs-lookup"><span data-stu-id="68fc0-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="68fc0-107">أضافه إعدادات البريد الكتروني لأجهزه iOS و إيبادوس في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="68fc0-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="68fc0-108">إعدادات ملف تعريف البريد الكتروني في Microsoft Intune للاجهزه التي تعمل بنظام Windows Phone 8.1</span><span class="sxs-lookup"><span data-stu-id="68fc0-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="68fc0-109">إعدادات ملف تعريف البريد الكتروني للاجهزه التي تعمل بنظام Windows 10 في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="68fc0-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="68fc0-110">**مشكله المزامنة الشائعة**</span><span class="sxs-lookup"><span data-stu-id="68fc0-110">**Common syncing issue**</span></span>

<span data-ttu-id="68fc0-111">**يحول كنوكس علي ملف تعريف البريد الكتروني لنظام التشغيل Android جات اتصال المستخدم والتقويم والمهام ، من المزامنة إلى أجهزه المستخدم.**</span><span class="sxs-lookup"><span data-stu-id="68fc0-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="68fc0-112">يعرض كنوكس علي ملف تعريف البريد الكتروني الذي يعمل بنظام التشغيل Android كنوكس المسؤول خيارا لتحديد أنواع المحتويات التي ستتم مزامنتها علي الجهاز بتعيين كل إلى تمكين.</span><span class="sxs-lookup"><span data-stu-id="68fc0-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="68fc0-113">إذا تم تعيين الاعداد لأي نوع من أنواع المحتويات إلى **غير مكون** (الافتراضي) ، فلن تتم مزامنة نوع المحتوي هذا تلقائيا.</span><span class="sxs-lookup"><span data-stu-id="68fc0-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="68fc0-114">قد يقوم المستخدم بتمكين نوع المحتوي الذي يريدونه مباشره علي الجهاز يدويا ، ولكن يتم الكتابة فوق هذا التكوين بواسطة اعداد نهج Intune ، وتتوقف المزامنة عن نوع المحتوي هذا.</span><span class="sxs-lookup"><span data-stu-id="68fc0-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

