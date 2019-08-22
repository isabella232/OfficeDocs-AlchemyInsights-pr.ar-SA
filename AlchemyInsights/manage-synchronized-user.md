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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36541968"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="2512e-102">غير قادر على تعيين عنوان البريد الإلكتروني الأساسي أو تغيير خصائص المستخدم</span><span class="sxs-lookup"><span data-stu-id="2512e-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="2512e-103">إذا تم تمكين مزامنة الدليل للبيئة الخاصة بك، يتعذر تغيير بعض خصائص المستخدم أو الكائن استخدام مركز مسؤول Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="2512e-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="2512e-104">لإدارة المستخدمين المتزامنة والسمات الخاصة بها بشكل كامل، استخدم الدليل النشط المحلي مستخدمين ومجموعات إدارة وحدة التحكم (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="2512e-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="2512e-105">بدلاً من ذلك، يمكنك تغيير المستخدمين الفرديين أو سمات للمستخدمين متزامنة باستخدام powershell مثل المعروضة في هذه الأمثلة الشائعة:</span><span class="sxs-lookup"><span data-stu-id="2512e-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="2512e-106">مجموعة مسولوسير user2@yourvanitydomain.onmicrosoft.com-التيرناتيمايلادريسيس user@yourdomain.onmicrosoft.com-UserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="2512e-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="2512e-107">مجموعة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com"-اسم العرض "اختبار المستخدم"-"اسم العائلة" "المستخدم"-العنوان "مدير"-قسم "الموارد البشرية"</span><span class="sxs-lookup"><span data-stu-id="2512e-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="2512e-108">إزالة مسولوسير-UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="2512e-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>