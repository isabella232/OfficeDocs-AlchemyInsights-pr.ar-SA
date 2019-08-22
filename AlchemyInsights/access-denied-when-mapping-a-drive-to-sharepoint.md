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
ms.openlocfilehash: c73358ebfbdede5b4e43ca2c35146f6611958e23
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36495846"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="6a59f-102">إصلاح مشاكل مكتبات SharePoint تعيين محركات أقراص الشبكة</span><span class="sxs-lookup"><span data-stu-id="6a59f-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="6a59f-103">عند قيامك بالاستعراض إلى محرك أقراص شبكة معين، قد ترى إحدى الرسائل التالية:</span><span class="sxs-lookup"><span data-stu-id="6a59f-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="6a59f-104">**\\مسار غير قابل للوصول. قد لا يكون لديك إذن لاستخدام مورد شبكة الاتصال هذا. اتصل بمسؤول الملقم لمعرفة ما إذا كان لديك أذونات الوصول.**</span><span class="sxs-lookup"><span data-stu-id="6a59f-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="6a59f-105">**تم رفض الوصول. قبل فتح الملفات في هذا الموقع، الذي يجب أولاً إضافة موقع ويب إلى قائمة المواقع الموثوق بها الخاصة بك استعراض موقع ويب وتحديد خيار تسجيل الدخول تلقائياً.**</span><span class="sxs-lookup"><span data-stu-id="6a59f-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="6a59f-106">[محركات أقراص الشبكة المعينة الحصول على المساعدة في استكشاف الأخطاء وإصلاحها](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span><span class="sxs-lookup"><span data-stu-id="6a59f-106">[Get help troubleshooting mapped network drives](https://support.office.com/article/ef399c67-4578-4c3a-adbe-0b489084eabe.aspx).</span></span>
  
<span data-ttu-id="6a59f-107">تعيين مكتبة كمحرك أقراص شبكة اتصال تم المؤقتة والمعتمدة فقط في Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="6a59f-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="6a59f-108">بدلاً من ذلك، [مزامنة الملفات SharePoint مع عميل المزامنة أندريف الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="6a59f-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="6a59f-109">الوصول إلى كافة الملفات في أندريف دون استخدام مساحة للتخزين المحلي.</span><span class="sxs-lookup"><span data-stu-id="6a59f-109">Access all your files in OneDrive without using local storage space.</span></span>
  