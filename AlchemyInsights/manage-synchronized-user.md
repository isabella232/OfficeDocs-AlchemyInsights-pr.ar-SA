---
title: إدارة مستخدم متزامن
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380492"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="8bddd-102">غير قادر على تعيين عنوان البريد الإلكتروني الأساسي أو تغيير خصائص المستخدم</span><span class="sxs-lookup"><span data-stu-id="8bddd-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="8bddd-103">إذا تم تمكين مزامنة الدليل للبيئة الخاصة بك لا تغيير بعض خصائص المستخدم أو الكائن استخدام مركز الإدارة.</span><span class="sxs-lookup"><span data-stu-id="8bddd-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="8bddd-104">لإدارة المستخدمين المتزامنة والسمات الخاصة بها بشكل كامل، استخدم الدليل النشط المحلي مستخدمين ومجموعات إدارة وحدة التحكم (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="8bddd-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="8bddd-105">بدلاً من ذلك، يمكنك تغيير المستخدمين الفرديين أو سمات للمستخدمين متزامنة باستخدام powershell مثل المعروضة في هذه الأمثلة الشائعة:</span><span class="sxs-lookup"><span data-stu-id="8bddd-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="8bddd-106">مجموعة مسولوسير user2@yourvanitydomain.onmicrosoft.com-التيرناتيمايلادريسيس user@yourdomain.onmicrosoft.com-UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8bddd-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="8bddd-107">مجموعة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com"-اسم العرض "اختبار المستخدم"-"اسم العائلة" "المستخدم"-العنوان "مدير"-قسم "الموارد البشرية"</span><span class="sxs-lookup"><span data-stu-id="8bddd-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="8bddd-108">إزالة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="8bddd-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>