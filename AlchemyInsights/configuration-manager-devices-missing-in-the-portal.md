---
title: أجهزة إدارة التكوين المفقودة في المدخل
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
- "4384"
ms.openlocfilehash: 7a11ad3c6970be2c52a7cf0696bd3810b9bd665a
ms.sourcegitcommit: 89ae9e8b36d1980f89f07b016fff0ec48f96b620
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/23/2020
ms.locfileid: "43789523"
---
# <a name="configuration-manager-devices-missing-in-the-portal"></a><span data-ttu-id="adebc-102">أجهزة إدارة التكوين المفقودة في المدخل</span><span class="sxs-lookup"><span data-stu-id="adebc-102">Configuration Manager devices missing in the portal</span></span>

<span data-ttu-id="adebc-103">لتمكين مزامنة الأجهزة، يجب أن تكون[نقاط النهاية عبر الإنترنت المطلوبة](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) سهلة الوصول من الخادم المحلي الذي يستضيف دور "نقطة اتصال الخدمة".</span><span class="sxs-lookup"><span data-stu-id="adebc-103">For device sync to work, [required internet endpoints](https://docs.microsoft.com/configmgr/tenant-attach/device-sync-actions#internet-endpoints) must be reachable from the on-premise server hosting the Service Connection Point role.</span></span> <span data-ttu-id="adebc-104">لاستكشاف أخطاء مزامنة الأجهزة وإصلاحها، رجاءً راجع **CMGatewaySyncUploadWorker.log** الموجود على نقطة اتصال الخدمة.</span><span class="sxs-lookup"><span data-stu-id="adebc-104">To troubleshoot device sync, please review the **CMGatewaySyncUploadWorker.log** located on the service connection point.</span></span>

<span data-ttu-id="adebc-105">تعرّف على المزيد حول [إرفاق المستأجر في إدارة نقاط النهاية من Microsoft](https://docs.microsoft.com/configmgr/tenant-attach/).</span><span class="sxs-lookup"><span data-stu-id="adebc-105">Learn more about [Tenant attach in Microsoft Endpoint Manager](https://docs.microsoft.com/configmgr/tenant-attach/).</span></span>
