---
title: رفض الوصول عند تعيين محرك أقراص إلى SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 8fc866390d63443c94beef76b6a53a628b85d6d2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668730"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="ca542-102">إصلاح المشاكل المتعلقة بمكتبات SharePoint المعينة لمحركات أقراص الشبكة</span><span class="sxs-lookup"><span data-stu-id="ca542-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="ca542-103">عند الاستعراض وصولا إلى محرك أقراص شبكه تم تعيينه ، قد تري أحدي الرسائل التالية:</span><span class="sxs-lookup"><span data-stu-id="ca542-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="ca542-104">**\\لا يمكن الوصول إلى المسار. قد لا يكون لديك الاذن لاستخدام مورد الشبكة هذا. اتصل بمسؤول هذا الخادم لمعرفه ما إذا كان لديك أذونات الوصول.**</span><span class="sxs-lookup"><span data-stu-id="ca542-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="ca542-105">**تم رفض الوصول. قبل فتح الملفات في هذا الموقع ، يجب أولا أضافه موقع ويب إلى قائمه الموقع الموثوق به ، والاستعراض وصولا إلى موقع ويب ، وتحديد خيار تسجيل الدخول تلقائيا.**</span><span class="sxs-lookup"><span data-stu-id="ca542-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="ca542-106">[الحصول علي المساعدة لاستكشاف أخطاء محركات أقراص الشبكة المعينة](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span><span class="sxs-lookup"><span data-stu-id="ca542-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="ca542-107">تعيين مكتبه كمحرك أقراص الشبكة مؤقتا ومعتمده في Internet Explorer فقط.</span><span class="sxs-lookup"><span data-stu-id="ca542-107">Mapping a library as a network drive is temporary and supported only in Internet Explorer.</span></span> <span data-ttu-id="ca542-108">بدلا من ذلك ، يمكنك [مزامنة ملفات SharePoint باستخدام عميل المزامنة من OneDrive الجديد](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) الذي يتضمن [الملفات عند الطلب](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span><span class="sxs-lookup"><span data-stu-id="ca542-108">Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx).</span></span> <span data-ttu-id="ca542-109">يمكنك الوصول إلى كل ملفاتك في OneDrive دون استخدام مساحة التخزين المحلية.</span><span class="sxs-lookup"><span data-stu-id="ca542-109">Access all your files in OneDrive without using local storage space.</span></span>
  