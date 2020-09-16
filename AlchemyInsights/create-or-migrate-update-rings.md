---
title: إنشاء حلقه تحديث أو ترحيلها
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1126"
- "6700007"
ms.openlocfilehash: 06f905551cbd015c80b6de4f97d0beb535d70fa0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732342"
---
# <a name="create-or-migrate-update-rings"></a><span data-ttu-id="9e9fb-102">إنشاء حلقه تحديث أو ترحيلها</span><span class="sxs-lookup"><span data-stu-id="9e9fb-102">Create or migrate update rings</span></span>

<span data-ttu-id="9e9fb-103">إذا قمت بتكوين إعدادات تحديث Windows 10 في مدخل Intune الكلاسيكي وكانت تريد ترحيل الإعدادات إلى Intune في مدخل Azure ، فاتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="9e9fb-103">If you configured Windows 10 update settings in the Intune classic portal and you want to migrate the settings to Intune in the Azure portal, follow these steps:</span></span>

1.  <span data-ttu-id="9e9fb-104">انتقل إلى مدخل Azure وحدد  **كل الخدمات**.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-104">Go to the Azure portal and select  **All Services**.</span></span>
2.  <span data-ttu-id="9e9fb-105">في حقل  **عامل التصفية**  ، اكتب  **Intune**، واختر  **Microsoft Intune**.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-105">In the  **Filter**  field, type  **Intune**, and choose  **Microsoft Intune**.</span></span>
3.  <span data-ttu-id="9e9fb-106">حدد **تحديثات البرامج**التي   >   تنشئها**الحلقات لتحديث Windows 10**   >   **Create**.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-106">Select  **Software updates**  >  **Windows 10 Update Rings**  >  **Create**.</span></span>
4.  <span data-ttu-id="9e9fb-107">ادخل اسما ووصفا ، وحدد  **تكوين**.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-107">Enter a name and description, and select  **Configure**.</span></span>
5.  <span data-ttu-id="9e9fb-108">قم بتكوين إعدادات تحديث البرنامج لمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-108">Configure the software update settings for your organization.</span></span>
6.  <span data-ttu-id="9e9fb-109">حدد **موافق**إنشاء  >  **رنين تحديث**  >  **Create**.</span><span class="sxs-lookup"><span data-stu-id="9e9fb-109">Select  **OK** > **Create Update Ring** > **Create**.</span></span>