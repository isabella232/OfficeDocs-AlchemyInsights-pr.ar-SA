---
title: تعيين SharePoint إلى محرك أقراص شبكة
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 741d22c4231886b385b0bc2361e429929ef58f4b84d56e51186f129fc5d07921
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/11/2021
ms.locfileid: "57901575"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>تعيين SharePoint إلى محرك أقراص شبكة

بدلا من تعيين محرك أقراص شبكة، SharePoint الملفات باستخدام المزامنة من OneDrive الجديد، الذي يوفر الملفات عند الطلب. يمكنك الوصول إلى جميع الملفات في OneDrive بدون استخدام مساحة السعة التخزينية المحلية. لمزيد من المعلومات، راجع [مزامنة](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) SharePoint الملفات Teams مع الكمبيوتر وتوفير مساحة على القرص باستخدام OneDrive عند الطلب [Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e).

إذا اخترت تعيين محرك أقراص بدلا من استخدام المزامنة من OneDrive [الجديد،](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)فتأكد من اتباع الخطوات التالية:

- [استكشاف أخطاء تعيين محركات أقراص الشبكة للاتصال بـ SharePoint Online](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [تحدث أخطاء المصادقة عندما لا يكون لدى العميل دعم TLS 1.2](https://docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**ملاحظة:** إذا كنت تستخدم Internet Explorer 10 مع Windows 8 أو Windows 7، وتلقيت رفض **الوصول** أو **لا** يمكن الوصول إلى Path عند تعيين محرك أقراص، فحل هذه المشكلة عن طريق تثبيت [هذه المشكلة.](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)