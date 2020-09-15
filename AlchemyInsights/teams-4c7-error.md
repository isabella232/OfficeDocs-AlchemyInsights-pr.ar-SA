---
title: خطا في الفرق 4 c7
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
- "3472"
- "9001211"
ms.openlocfilehash: 08494b461a24eba8999a5edb99c89af7b17db9b3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700190"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="bde13-102">خطا 4c7 في فرق Microsoft</span><span class="sxs-lookup"><span data-stu-id="bde13-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="bde13-103">يحدث هذا الخطا لان فرق Microsoft تتطلب مصادقه النماذج.</span><span class="sxs-lookup"><span data-stu-id="bde13-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="bde13-104">عند نشر خدمات الأمان المشترك ل Active directory (AD FS) ، لا يتم تمكين مصادقه النماذج لإنترانت بشكل افتراضي.</span><span class="sxs-lookup"><span data-stu-id="bde13-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="bde13-105">إذا فشلت عمليه المصادقة المتكاملة في Windows ، ستتم مطالبتك بتسجيل الدخول باستخدام مصادقه النماذج.</span><span class="sxs-lookup"><span data-stu-id="bde13-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="bde13-106">لحل هذه المشكلة ، قم بتمكين مصادقه النماذج باستخدام الاداه الاضافيه AD FS Console (MMC) علي الكمبيوتر الذي يحتوي علي النسخة المحلية من Active directory.</span><span class="sxs-lookup"><span data-stu-id="bde13-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="bde13-107">لعمل ذلك، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="bde13-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="bde13-108">في جزء التنقل ، استعرض بحثا عن **نهج المصادقة**.</span><span class="sxs-lookup"><span data-stu-id="bde13-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="bde13-109">ضمن **الإجراءات** في جزء التفاصيل ، حدد **تحرير المصادقة الاساسيه العامة**.</span><span class="sxs-lookup"><span data-stu-id="bde13-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="bde13-110">علي علامة التبويب **إنترانت** ، حدد **مصادقه النماذج**.</span><span class="sxs-lookup"><span data-stu-id="bde13-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="bde13-111">حدد **موافق** (أو **تطبيق**).</span><span class="sxs-lookup"><span data-stu-id="bde13-111">Select **OK** (or **Apply**).</span></span>