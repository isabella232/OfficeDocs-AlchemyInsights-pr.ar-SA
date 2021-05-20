---
title: تم إغلاق الاتصال الأساسي في SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: 0515ead28cdfdbdb9529c269b5170b294ab2b120
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543024"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a><span data-ttu-id="f505e-102">الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint</span><span class="sxs-lookup"><span data-stu-id="f505e-102">"The underlying connection was closed" error in SharePoint</span></span>

<span data-ttu-id="f505e-103">إذا كنت تتلقى الخطأ "تم إغلاق الاتصال الأساسي" في SharePoint فقد يكون مرتبطا ب إهمال TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="f505e-103">If you are receiving the error "The underlying connection was closed" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="f505e-104">لمزيد من المعلومات، راجع المقالات التالية:</span><span class="sxs-lookup"><span data-stu-id="f505e-104">For more info, see these articles:</span></span>

- [<span data-ttu-id="f505e-105">التحضير ل TLS 1.2 في Office 365 Office 365 سحابة القطاع الحكومي</span><span class="sxs-lookup"><span data-stu-id="f505e-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="f505e-106">تحدث أخطاء المصادقة إذا لم يكن لدى العميل دعم TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="f505e-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="f505e-107">تحديث لتمكين TLS 1.1 و TLS 1.2 كبروتوكولات آمنة افتراضية في WinHTTP في Windows</span><span class="sxs-lookup"><span data-stu-id="f505e-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="f505e-108">إذا كان المستخدمون Windows 7، فتأكد من التحقق من [مجموعات TLS Cipher في](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)Windows 7 .</span><span class="sxs-lookup"><span data-stu-id="f505e-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>