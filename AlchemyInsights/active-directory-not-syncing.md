---
title: لم تتم مزامنة active directory
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3517f424b4dcd89f915acebab747a9bff993fdbd
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47697616"
---
# <a name="active-directory-not-syncing"></a><span data-ttu-id="f1263-102">لم تتم مزامنة active directory</span><span class="sxs-lookup"><span data-stu-id="f1263-102">Active Directory not syncing</span></span>

<span data-ttu-id="f1263-103">إذا كنت تتلقي أخطاء مزامنة ، علي سبيل المثال "لا يوجد مزامنة حديثه" أو ملاحظه حاله مزامنة الدليل في مدخل مسؤول Office ، فهذا يعني ان هذا الAADConnect لديه إعدادات غير صحيحه أو أذونات غير كافيه لاجراء المزامنة.</span><span class="sxs-lookup"><span data-stu-id="f1263-103">If you are receiving synchronization errors, such as "no recent synchronization," or notice the directory synchronization status in the Office admin portal says, "Last synced more than 3 days ago," it may be that AADConnect has incorrect settings or insufficient permissions to perform a synchronization.</span></span>  

<span data-ttu-id="f1263-104">قد يؤدي أعاده تثبيت AADConnect باستخدام الإعدادات السريعة إلى حل المشكلة بسرعة:</span><span class="sxs-lookup"><span data-stu-id="f1263-104">Reinstalling AADConnect by using express settings may resolve the issue quickly:</span></span>

1. <span data-ttu-id="f1263-105">قم [بتنزيل أحدث إصدار من AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span><span class="sxs-lookup"><span data-stu-id="f1263-105">[Download the latest version of AADConnect](https://go.microsoft.com/fwlink/?LinkId=615771).</span></span>

2. <span data-ttu-id="f1263-106">[اتبع الإرشادات الخاصة بالتثبيت السريع](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span><span class="sxs-lookup"><span data-stu-id="f1263-106">[Follow the instructions for express installation](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express).</span></span>

<span data-ttu-id="f1263-107">لمزيد من المعلومات حول حسابات خدمات AADConnect ، راجع [AZURE AD Connect: الحسابات والأذونات](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span><span class="sxs-lookup"><span data-stu-id="f1263-107">For more information about AADConnect service accounts, see [Azure AD Connect: Accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions).</span></span>
