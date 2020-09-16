---
title: أعاده توجيه onedrive for Business علي ويب
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776366"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="e9d34-102">تمت أعاده التوجيه إلى Delve بعد النقر فوق OneDrive</span><span class="sxs-lookup"><span data-stu-id="e9d34-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="e9d34-103">راجع [دليل استكشاف الأخطاء وإصلاحها](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)المفصل.</span><span class="sxs-lookup"><span data-stu-id="e9d34-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="e9d34-104">لحل هذه المشكلة ، يجب ان يقوم المسؤول بمنح المستخدمين حق إنشاء موقع "المواقع الخاصة بي".</span><span class="sxs-lookup"><span data-stu-id="e9d34-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="e9d34-105">هذا بسبب إنشاء صفحه OneDrive for Business علي "المواقع الخاصة بي".</span><span class="sxs-lookup"><span data-stu-id="e9d34-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="e9d34-106">لمنح هذا الحق ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="e9d34-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="e9d34-107">في مركز أداره SharePoint ، انقر فوق **ملفات تعريف المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="e9d34-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="e9d34-108">في المقطع **الأشخاص** ، انقر فوق **أداره أذونات المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="e9d34-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="e9d34-109">أضف المستخدمين الذين يحتاجون إلى أذونات لإنشاء موقع "المواقع الخاصة بي".</span><span class="sxs-lookup"><span data-stu-id="e9d34-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="e9d34-110">بشكل افتراضي ، يتم تعيين هذا الاعداد إلى **الجميع باستثناء المستخدمين الخارجيين**.</span><span class="sxs-lookup"><span data-stu-id="e9d34-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="e9d34-111">بعد أضافه المستخدم أو المستخدمين أو المجموعة ، تاكد من تحديد المستخدم أو المستخدمون أو المجموعة التي تمت اضافتها ، وقم بالتمرير إلى المقطع **أذونات** ، ثم حدد خانه الاختيار الموجودة إلى جانب **إنشاء موقع شخصي (مطلوب للتخزين الشخصي وملف الاخبار والمحتوي المتبع)**.</span><span class="sxs-lookup"><span data-stu-id="e9d34-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="e9d34-112">انقر فوق **موافق**، ثم اجعل المستخدم يستعرض صفحه OneDrive لإنشاء الموقع.</span><span class="sxs-lookup"><span data-stu-id="e9d34-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
