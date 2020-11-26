---
title: إعدادات نهج حماية تطبيق Android في Microsoft Intune
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003997"
- "7057"
ms.openlocfilehash: 327df6e0a901037cd929cb845f805466d9bd4eff
ms.sourcegitcommit: 81c86027933c06db08d264918f2698d9c9a1659a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/20/2020
ms.locfileid: "49447200"
---
# <a name="android-app-protection-policy-settings-in-microsoft-intune"></a><span data-ttu-id="6c71a-102">إعدادات نهج حماية تطبيق Android في Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="6c71a-102">Android app protection policy settings in Microsoft Intune</span></span>

<span data-ttu-id="6c71a-103">هناك ثلاث فئات من إعدادات نهج حماية التطبيق للاجهزه التي تعمل بنظام Android:</span><span class="sxs-lookup"><span data-stu-id="6c71a-103">There are three categories of app protection policy settings for Android devices:</span></span>

<span data-ttu-id="6c71a-104">تتحكم **حماية البيانات** في كيفيه التعامل مع بيانات الشركة ، علي سبيل المثال ، ما إذا كان بالإمكان نسخ البيانات أو لصقها إلى تطبيق مختلف أو ما إذا كان من الممكن نقل لقطه شاشه من التطبيق.</span><span class="sxs-lookup"><span data-stu-id="6c71a-104">**Data protection** controls how company data is handled, such as, whether data can be copied or pasted to a different app or whether a screenshot can be taken of the app.</span></span> <span data-ttu-id="6c71a-105">تقوم الإعدادات أيضا بفرض التشفير علي بيانات الشركة وأداره ما إذا كان بالإمكان مزامنة بعض البيانات مع تطبيقات الجهاز الاصليه ، مثل قائمه جات الاتصال أو مستعرض ويب.</span><span class="sxs-lookup"><span data-stu-id="6c71a-105">The settings also enforce encryption on company data and manage whether certain data can be synced with the native device apps, like the contact list or web browser.</span></span> <span data-ttu-id="6c71a-106">لمعرفه المزيد ، راجع [حماية البيانات](https://go.microsoft.com/fwlink/?linkid=2135259).</span><span class="sxs-lookup"><span data-stu-id="6c71a-106">To learn more, see [Data protection](https://go.microsoft.com/fwlink/?linkid=2135259).</span></span>

<span data-ttu-id="6c71a-107">ترشد **متطلبات Access** كيفيه وصول المستخدمين إلى أحد التطبيقات.</span><span class="sxs-lookup"><span data-stu-id="6c71a-107">**Access requirements** guides how users can access an app.</span></span> <span data-ttu-id="6c71a-108">علي سبيل المثال ، قد يتطلب تطبيق المستخدم إدخال رقم PIN أو بصمه اصبع للوصول اليه.</span><span class="sxs-lookup"><span data-stu-id="6c71a-108">For example, an app could require the user to enter a PIN or fingerprint to access it.</span></span> <span data-ttu-id="6c71a-109">لمعرفه المزيد ، راجع [متطلبات الوصول](https://go.microsoft.com/fwlink/?linkid=2135260).</span><span class="sxs-lookup"><span data-stu-id="6c71a-109">To learn more, see [Access requirements](https://go.microsoft.com/fwlink/?linkid=2135260).</span></span>

<span data-ttu-id="6c71a-110">تحكم **التشغيل الشرطي** بإعدادات أمان تسجيل الدخول لتطبيق ما ، مثل ، الحد الأقصى لعدد مرات التثبيت قبل التامين أو الحد الأدنى المطلوب لنظام التشغيل لتشغيل التطبيق.</span><span class="sxs-lookup"><span data-stu-id="6c71a-110">**Conditional launch** governs the sign-in security settings for an app, such as, the maximum PIN attempts before lockout or the minimum operating system needed to run the app.</span></span> <span data-ttu-id="6c71a-111">لمعرفه المزيد ، راجع [التشغيل الشرطي](https://go.microsoft.com/fwlink/?linkid=2135507).</span><span class="sxs-lookup"><span data-stu-id="6c71a-111">To learn more, see [Conditional launch](https://go.microsoft.com/fwlink/?linkid=2135507).</span></span>
