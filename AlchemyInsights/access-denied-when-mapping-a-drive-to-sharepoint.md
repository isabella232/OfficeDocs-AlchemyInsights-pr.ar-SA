---
title: تم رفض الوصول عند تعيين محرك أقراص إلى SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 12/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: c41bfd9d25c8aa946a4ec5156be6d2424f4e2133
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/18/2019
ms.locfileid: "36737464"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="ed501-102">إصلاح مشاكل مع مكتبات SharePoint المعينة إلى محركات أقراص الشبكة</span><span class="sxs-lookup"><span data-stu-id="ed501-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="ed501-103">عند الاستعراض إلى محرك أقراص شبكه معين قد تري أحدي الرسائل التالية:</span><span class="sxs-lookup"><span data-stu-id="ed501-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="ed501-104">**\\المسار غير قابل للوصول. قد لا يكون لديك الاذن باستخدام مورد شبكه الاتصال هذا. اتصل بمسؤول هذا الملقم لمعرفه ما إذا كان لديك أذونات الوصول.**</span><span class="sxs-lookup"><span data-stu-id="ed501-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="ed501-105">**تم رفض الوصول. قبل فتح الملفات في هذا الموقع ، يجب أولا أضافه موقع ويب إلى قائمه المواقع الموثوق بها ، والاستعراض إلى موقع الويب ، وتحديد الخيار لتسجيل الدخول تلقائيا.**</span><span class="sxs-lookup"><span data-stu-id="ed501-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="ed501-106">[الحصول علي تعليمات استكشاف أخطاء محركات أقراص الشبكة المعينة](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="ed501-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="ed501-107">تعيين مكتبه كمحرك أقراص شبكه مؤقت ومعتمد فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="ed501-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="ed501-108">بدلا من ذلك ، [مزامنة ملفات SharePoint مع عميل المزامنة اندريف الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="ed501-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="ed501-109">الوصول إلى كافة الملفات الخاصة بك في OneDrive دون استخدام مساحة التخزين المحلية.</span><span class="sxs-lookup"><span data-stu-id="ed501-109">Access all your files in OneDrive without using local storage space.</span></span>
  