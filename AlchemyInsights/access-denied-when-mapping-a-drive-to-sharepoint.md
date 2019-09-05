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
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737464"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="878f0-102">إصلاح المشاكل المتعلقة بمكتبات SharePoint المعينة إلى محركات أقراص الشبكة</span><span class="sxs-lookup"><span data-stu-id="878f0-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="878f0-103">عند استعراض إلى محرك أقراص شبكة معين قد تشاهد إحدى الرسائل التالية:</span><span class="sxs-lookup"><span data-stu-id="878f0-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="878f0-104">**\\المسار غير قابل للوصول. قد لا يكون لديك الإذن لاستخدام مورد شبكة الاتصال هذا. اتصل بمسؤول هذا الملقم لمعرفة ما إذا كان لديك أذونات الوصول.**</span><span class="sxs-lookup"><span data-stu-id="878f0-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="878f0-105">**تم رفض الوصول. قبل فتح الملفات في هذا الموقع، يجب أولاً إضافة موقع ويب إلى قائمة المواقع الموثوق بها، والاستعراض إلى موقع ويب، وتحديد خيار تسجيل الدخول تلقائيًا.**</span><span class="sxs-lookup"><span data-stu-id="878f0-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="878f0-106">[الحصول على تعليمات استكشاف أخطاء محركات أقراص الشبكة المعينة وإصلاحها](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="878f0-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="878f0-107">تعيين مكتبة كمحرك أقراص شبكة مؤقتة ومعتمدة فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="878f0-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="878f0-108">بدلاً من ذلك، [قم بمزامنة ملفات SharePoint مع عميل المزامنة OneDrive الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="878f0-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="878f0-109">الوصول إلى كافة الملفات الخاصة بك في أندريف دون استخدام مساحة التخزين المحلية.</span><span class="sxs-lookup"><span data-stu-id="878f0-109">Access all your files in OneDrive without using local storage space.</span></span>
  