---
title: الترحيل إلى SharePoint Online بواسطة "إدارة الترحيل"
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931777"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="02a17-102">الترحيل إلى SharePoint Online بواسطة "إدارة الترحيل"</span><span class="sxs-lookup"><span data-stu-id="02a17-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="02a17-103">**هام**: يقوم العديد من عملاء SharePoint Online وOneDrive بتشغيل تطبيقات هامة للأعمال بالتوازي مع الخدمات التي يتم تشغيلها في الخلفية.</span><span class="sxs-lookup"><span data-stu-id="02a17-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="02a17-104">حيث تتضمن ترحيل المحتوى وتفادي فقدان البيانات (DLP) وحلول النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="02a17-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="02a17-105">خلال هذه الأوقات غير المسبوقة، سنقوم باتخاذ الخطوات التالية لضمان بقاء خدمات SharePoint Online و OneDrive متوفرة على مستوى عالٍ من الجودة والوثوقية للمستخدمين الذين يعتمدون على تلك الخدمات أكثر من ذي قبل في سيناريوهات العمل عن بُعد.</span><span class="sxs-lookup"><span data-stu-id="02a17-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="02a17-106">لدعم هذا الهدف، قمنا بتطبيق تقييد أكبر على التطبيقات الخلفية (الترحيل وتفادي فقدان البيانات (DLP) وحلول النسخ الاحتياطي) خلال ساعات النهار من أيام العمل.</span><span class="sxs-lookup"><span data-stu-id="02a17-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="02a17-107">يجب أن تضع في حسبانك أن هذه التطبيقات سيكون معدل نقلها محدوداً جداً خلال هذه الأوقات.</span><span class="sxs-lookup"><span data-stu-id="02a17-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="02a17-108">وعلى الرغم من ذلك، ستكون الخدمة جاهزة لمعالجة حجم أكبر من طلبات التطبيقات الخلفية أثناء المساء وساعات نهاية الأسبوع في منطقتك.</span><span class="sxs-lookup"><span data-stu-id="02a17-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="02a17-109">**إدارة الترحيل**</span><span class="sxs-lookup"><span data-stu-id="02a17-109">**Migration Manager**</span></span>

<span data-ttu-id="02a17-110">ترشدك إدارة الترحيل خلال إعداد العملاء وإنشاء المهام، وتوجد في مركز إدارة SharePoint الحديث.</span><span class="sxs-lookup"><span data-stu-id="02a17-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="02a17-111">يمكنك تحديد الإعدادات العامة أو الخاصة بمستوي المهام وعرض تقدم المهام بشكل كامل، وتنزيل الملخصات المجمعة والتقارير على مستوى المهام.</span><span class="sxs-lookup"><span data-stu-id="02a17-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="02a17-112">بدء استخدام "إدارة الترحيل"</span><span class="sxs-lookup"><span data-stu-id="02a17-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="02a17-113">إعداد عملاء إدارة الترحيل</span><span class="sxs-lookup"><span data-stu-id="02a17-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="02a17-114">إعدادات إدارة الترحيل</span><span class="sxs-lookup"><span data-stu-id="02a17-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
