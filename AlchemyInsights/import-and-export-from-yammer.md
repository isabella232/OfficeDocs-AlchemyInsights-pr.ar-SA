---
title: الاستيراد والتصدير من Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034792"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="1412c-102">الاستيراد والتصدير من Yammer</span><span class="sxs-lookup"><span data-stu-id="1412c-102">Import and export from Yammer</span></span>

<span data-ttu-id="1412c-103">**استيراد**</span><span class="sxs-lookup"><span data-stu-id="1412c-103">**Import**</span></span>

<span data-ttu-id="1412c-104">تختلف خيارات استيراد المستخدم استنادا إلى ما إذا كانت Yammer الشبكة في الوضع الأصلي [ل Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)أو لا.</span><span class="sxs-lookup"><span data-stu-id="1412c-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="1412c-105">**الوضع غير** الأصلي : يمكن استيراد المستخدمين إلى مجموعات باستخدام إضافة من دفتر العنوان [(حد](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 100 [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) مستخدم) ضمن إعدادات المجموعة، أو إلى الشبكة باستخدام التحديث المجمع داخل مسؤول الشبكة.</span><span class="sxs-lookup"><span data-stu-id="1412c-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="1412c-106">**الوضع الأصلي**: يجب تنفيذ عمليات عضوية المجموعة وعضوية الشبكة من مدخل [مسؤول Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)، مدخل [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)، أو باستخدام خيار Azure AD آخر.</span><span class="sxs-lookup"><span data-stu-id="1412c-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="1412c-107">لم تعد الشبكات في الوضع الأصلي قادرة على الوصول إلى التحديث المجمع والميزات القديمة الأخرى.</span><span class="sxs-lookup"><span data-stu-id="1412c-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="1412c-108">Yammer أي دعم لاستيراد محتوى من داخل مسؤول الشبكة حتى عند استخدام ميزة "تصدير البيانات" في شبكة أخرى.</span><span class="sxs-lookup"><span data-stu-id="1412c-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="1412c-109">يمكن إعادة نشر المحتوى بواسطة حلول الشركاء أو Yammer واجهات برمجة التطبيقات REST.</span><span class="sxs-lookup"><span data-stu-id="1412c-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="1412c-110">**تصدير**</span><span class="sxs-lookup"><span data-stu-id="1412c-110">**Export**</span></span>

<span data-ttu-id="1412c-111">[يسمح تصدير بيانات الشبكة ضمن مسؤول](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) الشبكة بتصدير المحتوى من Yammer، بما في ذلك الرسائل والملفات.</span><span class="sxs-lookup"><span data-stu-id="1412c-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="1412c-112">يمكن أن تكون المرفقات كبيرة جدا وستتسبب في أن تستغرق عمليات التصدير وقتا طويلا لإكمالها.</span><span class="sxs-lookup"><span data-stu-id="1412c-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="1412c-113">نوصي بتصدير الشبكات النشطة باستخدام [API لتصدير](https://developer.yammer.com/docs/data-export-api) البيانات في أجزاء حسب اليوم أو الأسبوع.</span><span class="sxs-lookup"><span data-stu-id="1412c-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="1412c-114">لا يوفر دعم Microsoft برامج نصية مخصصة لهذا الغرض.</span><span class="sxs-lookup"><span data-stu-id="1412c-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="1412c-115">يوجد تصدير [القانون العام لحماية البيانات (GDPR)](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) منفصل لتصدير المحتوى لمستخدم فردي.</span><span class="sxs-lookup"><span data-stu-id="1412c-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>