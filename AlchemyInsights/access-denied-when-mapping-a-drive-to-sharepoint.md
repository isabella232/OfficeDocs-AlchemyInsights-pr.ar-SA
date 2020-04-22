---
title: تم رفض الوصول عند تعيين محرك أقراص إلى SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687353"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="44b5b-102">إصلاح المشاكل المتعلقة بمكتبات SharePoint التي تم تعيينها إلى محركات أقراص الشبكة</span><span class="sxs-lookup"><span data-stu-id="44b5b-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="44b5b-103">عند الاستعراض إلى محرك أقراص شبكة معينة، قد تشاهد إحدى الرسائل التالية:</span><span class="sxs-lookup"><span data-stu-id="44b5b-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="44b5b-104">**\\لا يمكن الوصول إلى المسار. قد لا يكون لديك إذن لاستخدام مورد الشبكة هذا. اتصل بمسؤول هذا الخادم لمعرفة ما إذا كان لديك أذونات وصول.**</span><span class="sxs-lookup"><span data-stu-id="44b5b-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="44b5b-105">**تم رفض الوصول. قبل فتح الملفات في هذا الموقع، يجب أولاً إضافة موقع ويب إلى قائمة الموقع الموثوق بها، والاستعراض إلى موقع ويب، وتحديد خيار تسجيل الدخول تلقائيًا.**</span><span class="sxs-lookup"><span data-stu-id="44b5b-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="44b5b-106">[الحصول على تعليمات استكشاف محركات أقراص الشبكة المعينة وإصلاحها](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="44b5b-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="44b5b-107">تعيين مكتبة كمحرك أقراص شبكة اتصال مؤقت ومعتمد فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="44b5b-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="44b5b-108">بدلاً من ذلك، [مزامنة ملفات SharePoint مع عميل مزامنة OneDrive الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="44b5b-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="44b5b-109">الوصول إلى جميع الملفات الخاصة بك في OneDrive دون استخدام مساحة التخزين المحلية.</span><span class="sxs-lookup"><span data-stu-id="44b5b-109">Access all your files in OneDrive without using local storage space.</span></span>
  