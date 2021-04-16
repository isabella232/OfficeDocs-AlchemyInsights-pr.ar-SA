---
title: OneDrive for Business Web OneDrive يعيد التوجيه إلى Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799976"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a><span data-ttu-id="c164d-102">تمت إعادة التوجيه إلى Delve بعد النقر فوق OneDrive</span><span class="sxs-lookup"><span data-stu-id="c164d-102">Redirected to Delve after you click OneDrive</span></span>

<span data-ttu-id="c164d-103">راجع دليل [استكشاف الأخطاء وإصلاحها التفصيلي.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)</span><span class="sxs-lookup"><span data-stu-id="c164d-103">See our detailed [Troubleshooting Guide](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).</span></span>

<span data-ttu-id="c164d-104">لحل هذه المشكلة، يجب على المسؤول منح المستخدمين الحق في إنشاء موقع "المواقع الخاصة بهم".</span><span class="sxs-lookup"><span data-stu-id="c164d-104">To resolve this problem, the administrator must grant users the right to create their My Sites site.</span></span> <span data-ttu-id="c164d-105">وذلك لأن صفحة OneDrive for Business تم إنشاؤها على "المواقع الخاصة".</span><span class="sxs-lookup"><span data-stu-id="c164d-105">This is because the OneDrive for Business page is created on My Sites.</span></span>

<span data-ttu-id="c164d-106">لمنح هذا الحق، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="c164d-106">To grant this right, follow these steps:</span></span>

1. <span data-ttu-id="c164d-107">في مركز إدارة SharePoint، انقر فوق **ملفات تعريف المستخدمين**.</span><span class="sxs-lookup"><span data-stu-id="c164d-107">In the SharePoint admin center,click **user profiles**.</span></span>

2. <span data-ttu-id="c164d-108">في المقطع **الأشخاص،** انقر فوق **إدارة أذونات المستخدم**.</span><span class="sxs-lookup"><span data-stu-id="c164d-108">In the **People** section, click **Manage User Permissions**.</span></span>

3. <span data-ttu-id="c164d-109">أضف المستخدمين الذين يحتاجون إلى أذونات لإنشاء موقع المواقع الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="c164d-109">Add users who require permissions to create their My Sites site.</span></span> <span data-ttu-id="c164d-110">بشكل افتراضي، يتم تعيين هذا الإعداد إلى **الجميع باستثناء المستخدمين الخارجيين**.</span><span class="sxs-lookup"><span data-stu-id="c164d-110">By default, this setting is set to **Everyone except external users**.</span></span>

4. <span data-ttu-id="c164d-111">بعد إضافة المستخدم أو المستخدمين أو المجموعة، تأكد من تحديد المستخدم أو المستخدمين أو  المجموعة المضافة، قم بالتمرير إلى مقطع الأذونات، ثم حدد خانة الاختيار بجانب إنشاء موقع شخصي (مطلوب للتخزين الشخصي وملف الأخبار والمحتوى الذي **يليه).**</span><span class="sxs-lookup"><span data-stu-id="c164d-111">After you have added the user, users, or group, make sure that the added user, users, or group is selected, scroll to the **permissions** section, and then select the check box next to **Create Personal Site (required for personal storage, newsfeed, and followed content)**.</span></span>

5. <span data-ttu-id="c164d-112">انقر **فوق** موافق ، ثم اسمح للمستخدم بالاستعراض إلى صفحة OneDrive لإنشاء الموقع.</span><span class="sxs-lookup"><span data-stu-id="c164d-112">Click **OK**, and then have the user browse to the OneDrive page to create the site.</span></span>
