---
title: وراثة الأذونات
ms.author: mikeplum
author: MikePlumleyMSFT
manager: scotv
ms.date: 8/7/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bb5c440a-ca70-4dc6-b517-688e80551101
ms.openlocfilehash: 5a72a74710a01cf958fa468b80ee67a4034c4383
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/22/2019
ms.locfileid: "30752189"
---
# <a name="how-permissions-inheritance-works-in-sharepoint"></a><span data-ttu-id="23ebc-102">كيف يعمل توريث الأذونات في SharePoint</span><span class="sxs-lookup"><span data-stu-id="23ebc-102">How permissions inheritance works in SharePoint</span></span>

<span data-ttu-id="23ebc-103">بشكل افتراضي، يتم توريث الأذونات في SharePoint من أعلى أعلى في التسلسل الهرمي.</span><span class="sxs-lookup"><span data-stu-id="23ebc-103">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="23ebc-104">لذا ملف يرث أذوناته من المجلد يرث أذوناته من المكتبة، يرث أذوناته من الموقع الذي يرث أذوناته من مجموعة الموقع.</span><span class="sxs-lookup"><span data-stu-id="23ebc-104">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site, which inherits its permissions from the site collection.</span></span>
  
<span data-ttu-id="23ebc-105">للحصول على مزيد من المعلومات حول إزالة أذونات فريدة واستعادة الوراثة، راجع [تحرير واداره الأذونات لقائمة أو مكتبة](https://go.microsoft.com/fwlink/?linkid=869946).</span><span class="sxs-lookup"><span data-stu-id="23ebc-105">For info about removing unique permissions and restoring inheritance, see [Edit and manage permissions for a list or library](https://go.microsoft.com/fwlink/?linkid=869946).</span></span>
  

