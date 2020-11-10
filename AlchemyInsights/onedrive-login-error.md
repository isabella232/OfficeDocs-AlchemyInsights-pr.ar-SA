---
title: AADSTS50011 خطا تسجيل الدخول إلى OneDrive
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982416"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="11d41-102">AADSTS50011 خطا تسجيل الدخول إلى OneDrive</span><span class="sxs-lookup"><span data-stu-id="11d41-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="11d41-103">إذا تلقيت رسالة الخطا "AADSTS50011: لا يتطابق عنوان URL المحدد في الطلب مع الرد" عند تسجيل الدخول إلى تطبيق OneDrive ، تحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="11d41-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="11d41-104">يجب ان يكون إصدار OneDrive الخاص بك مساويا للإصدار 20.052 أو أكبر منه. XXXX.</span><span class="sxs-lookup"><span data-stu-id="11d41-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="11d41-105">للتحقق من الإصدار الذي قمت به ، انقر فوق أيقونه OneDrive الزرقاء في منطقه الاعلام ، حدد **تعليمات & إعدادات > الإعدادات > حول**.</span><span class="sxs-lookup"><span data-stu-id="11d41-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="11d41-106">قد تحظر الشبكة نقل البيانات إلى **g.live.com** و **oneclient.sfx.ms**.</span><span class="sxs-lookup"><span data-stu-id="11d41-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="11d41-107">إذا تم حظر نقل البيانات ، فلن يتمكن OneDrive من تحديث نفسه.</span><span class="sxs-lookup"><span data-stu-id="11d41-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="11d41-108">استخدام مسؤول الشبكة لضمان امكانيه الوصول إلى عناوين Url هذه.</span><span class="sxs-lookup"><span data-stu-id="11d41-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="11d41-109">يجب ان تكون [نقاط النهاية هذه](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) يمكن الوصول اليها للعملاء الذين يستخدمون خطط Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="11d41-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="11d41-110">إذا كنت بحاجه إلى الحصول علي إصدار حالي من OneDrive يدويا ، فقم بزيارة [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="11d41-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
