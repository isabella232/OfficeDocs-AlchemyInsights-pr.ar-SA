---
title: حظر تواقيع البريد الإلكتروني التي من قبل المستخدم
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: dab7eacb617c8f3a8bd63634e974166b6e448d75
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480890"
---
# <a name="block-user-made-email-signatures"></a><span data-ttu-id="fbc7f-102">حظر تواقيع البريد الإلكتروني التي من قبل المستخدم</span><span class="sxs-lookup"><span data-stu-id="fbc7f-102">Block user-made email signatures</span></span>

<span data-ttu-id="fbc7f-103">ينطبق الحل التالي فقط على تواقيع البريد الإلكتروني التي تم إنشاؤها في Outlook على الويب.</span><span class="sxs-lookup"><span data-stu-id="fbc7f-103">The following solution only applies to email signatures created in Outlook on the web.</span></span> <span data-ttu-id="fbc7f-104">يمكنك حظر التواقيع في تطبيق Outlook فقط إذا كان لديك Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="fbc7f-104">You can only block signatures in the Outlook app if you have an on-premises Exchange Server.</span></span>

1. <span data-ttu-id="fbc7f-105">في مركز الإدارة، اختر **مراكز**  >  **الإدارة Exchange.**</span><span class="sxs-lookup"><span data-stu-id="fbc7f-105">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="fbc7f-106">انقر **فوق أذونات**  >  **سياسات Outlook Web App.**</span><span class="sxs-lookup"><span data-stu-id="fbc7f-106">Click **permissions** > **Outlook Web App policies**.</span></span>
3. <span data-ttu-id="fbc7f-107">حدد النهج، ثم انقر فوق أيقونة القلم الرصاص لتحريره.</span><span class="sxs-lookup"><span data-stu-id="fbc7f-107">Select the policy, and then click the pencil icon to edit it.</span></span>
4. <span data-ttu-id="fbc7f-108">انقر **فوق خيارات** إضافية  >  **للميزات.**</span><span class="sxs-lookup"><span data-stu-id="fbc7f-108">Click **features** > **More options**.</span></span>
5. <span data-ttu-id="fbc7f-109">ضمن **تجربة المستخدم،** قم بمسح خانة **الاختيار "توقيع** البريد الإلكتروني"، ثم انقر فوق **"حفظ".**</span><span class="sxs-lookup"><span data-stu-id="fbc7f-109">Under **User experience**, clear the **Email signature** check box, and then click **Save**.</span></span>

<span data-ttu-id="fbc7f-110">**هام:** إذا تم إضافة توقيع قبل مسح خانة الاختيار هذه، سيبقى المستخدم قادرا على استخدامه.</span><span class="sxs-lookup"><span data-stu-id="fbc7f-110">**Important:** If a signature was added before clearing this check box, the user will still be able to use it.</span></span> <span data-ttu-id="fbc7f-111">اطلب منه إزالته.</span><span class="sxs-lookup"><span data-stu-id="fbc7f-111">Ask them to remove it.</span></span>
