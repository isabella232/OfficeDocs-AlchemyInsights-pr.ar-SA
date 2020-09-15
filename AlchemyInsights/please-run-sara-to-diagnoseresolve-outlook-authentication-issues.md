---
title: 182 الرجاء تشغيل SaRA لتشخيص مشاكل مصادقه Outlook وحلها
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "182"
- "1800012"
ms.assetid: a3a5ea91-6989-4616-9290-c7b24484e8c8
ms.openlocfilehash: aa1e831eac829f3bd35f34e2fbe34923c5af0d3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47802008"
---
# <a name="use-sara-to-diagnose-and-resolve-outlook-authentication-issues"></a><span data-ttu-id="c1129-102">استخدام SaRA لتشخيص المشاكل المتعلقة بمصادقة Outlook وحلها</span><span class="sxs-lookup"><span data-stu-id="c1129-102">Use SaRA to diagnose and resolve Outlook authentication issues</span></span>

<span data-ttu-id="c1129-103">**ملاحظه**: يرجى التحقق لمعرفه ما إذا كان [الاعداد الافتراضي للامان](https://aka.ms/securitydefaults) ممكنا لمؤسسك.</span><span class="sxs-lookup"><span data-stu-id="c1129-103">**Note**: Please check to see whether [security defaults](https://aka.ms/securitydefaults) is enabled for your organization.</span></span> <span data-ttu-id="c1129-104">إذا تم إنشاء المستاجر بعد 21 أكتوبر ، 2019 وكان Outlook يطلب منك بشكل متكرر كلمه مرور ، فقد يكون لديك **افتراضيات أمان** ممكنة في نطاق المستاجر.</span><span class="sxs-lookup"><span data-stu-id="c1129-104">If your tenant was created after October 21st, 2019 and your Outlook is repeatedly asking you for a password, you may have **security defaults** enabled in your tenant.</span></span>

<span data-ttu-id="c1129-105">نوصي بشده باستخدام [Outlook للمطالبة بالرجوع إلى "تشخيص كلمه المرور](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) " علي الجهاز المتاثر لاستكشاف الأخطاء وإصلاحها حيث يطالب Outlook باستمرار بكلمه مرور.</span><span class="sxs-lookup"><span data-stu-id="c1129-105">We highly recommend you use the [Outlook keeps asking for my password](https://aka.ms/SaRA-OutlookPwdPrompt-Alchemy) diagnostic on the affected machine to troubleshoot issues where Outlook continually prompts for a password.</span></span> <span data-ttu-id="c1129-106">يقوم تشخيص [SaRA](https://diagnostics.office.com/#/) هذا بالتحقق من الحلول التي يمكنك استخدامها لمعالجه اي مشاكل تم اكتشافها.</span><span class="sxs-lookup"><span data-stu-id="c1129-106">This [SaRA](https://diagnostics.office.com/#/) diagnostic does automated checks and returns possible solutions for you to use to address any detected issues.</span></span>
