---
title: خطأ في Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786656"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="def73-102">خطأ 4c7 في Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="def73-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="def73-103">يحدث هذا الخطأ لأن Microsoft Teams يتطلب مصادقة النماذج.</span><span class="sxs-lookup"><span data-stu-id="def73-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="def73-104">عند نشر خدمات اتحاد Active Directory (AD FS)، لا يتم تمكين مصادقة النماذج للانترانت بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="def73-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="def73-105">إذا فشلت المصادقة المتكاملة ل Windows، فيطلب منك تسجيل الدخول باستخدام مصادقة النماذج.</span><span class="sxs-lookup"><span data-stu-id="def73-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="def73-106">لحل هذه المشكلة، قم بتمكين مصادقة النماذج باستخدام محاذاة وحدة تحكم إدارة AD FS (MMC) على الكمبيوتر الذي لديه النسخة المحلية من Active Directory.</span><span class="sxs-lookup"><span data-stu-id="def73-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="def73-107">لعمل ذلك، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="def73-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="def73-108">في جزء التنقل، استعرض بحثا عن **"سياسات المصادقة".**</span><span class="sxs-lookup"><span data-stu-id="def73-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="def73-109">ضمن **إجراءات** في جزء التفاصيل، حدد **تحرير المصادقة الأساسية العالمية**.</span><span class="sxs-lookup"><span data-stu-id="def73-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="def73-110">على علامة **التبويب إنترانت،** حدد **مصادقة النماذج**.</span><span class="sxs-lookup"><span data-stu-id="def73-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="def73-111">حدد **موافق** (أو **تطبيق).**</span><span class="sxs-lookup"><span data-stu-id="def73-111">Select **OK** (or **Apply**).</span></span>