---
title: الفرق 4c7 خطا
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 0945a341c6456ee4178c0485f3bfb9232fa78a11
ms.sourcegitcommit: 802537a54ef8bde1bdd758ee9a60b6c19d37d6e1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/19/2019
ms.locfileid: "40795928"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="0a0c0-102">خطا 4c7 في فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="0a0c0-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="0a0c0-103">يحدث هذا الخطا لان "فرق Microsoft" تتطلب "مصادقه النماذج".</span><span class="sxs-lookup"><span data-stu-id="0a0c0-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="0a0c0-104">عند نشر "خدمات الاتحاد خدمه Active Directory" (AD FS) ، لم يتم تمكين "مصادقه النماذج" لإنترانت بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="0a0c0-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="0a0c0-105">في حاله فشل "المصادقة المتكاملة ل Windows" ، تتم مطالبتك بتسجيل الدخول باستخدام "مصادقه النماذج".</span><span class="sxs-lookup"><span data-stu-id="0a0c0-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="0a0c0-106">لحل هذه المشكلة ، تمكين "مصادقه النماذج" باستخدام الاداه الاضافيه AD FS التحكم بالاداره ل Microsoft (MMC) علي الكمبيوتر الذي يحتوي علي النسخة المحلية من "Active Directory".</span><span class="sxs-lookup"><span data-stu-id="0a0c0-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="0a0c0-107">لعمل ذلك، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0a0c0-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="0a0c0-108">في جزء التنقل ، استعرض إلى **نهج المصادقة**.</span><span class="sxs-lookup"><span data-stu-id="0a0c0-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="0a0c0-109">ضمن **الإجراءات** الواردة في جزء التفاصيل ، حدد **تحرير المصادقة الاساسيه العمومية**.</span><span class="sxs-lookup"><span data-stu-id="0a0c0-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="0a0c0-110">ضمن علامة التبويب **إنترانت** ، حدد **مصادقه النماذج**.</span><span class="sxs-lookup"><span data-stu-id="0a0c0-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="0a0c0-111">حدد **موافق** (أو **تطبيق**).</span><span class="sxs-lookup"><span data-stu-id="0a0c0-111">Select **OK** (or **Apply**).</span></span>