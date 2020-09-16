---
title: لا تظهر تسميات الحساسية
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 6a64e001be115c8e5553a0d8c97b8cb815922c69
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47801171"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="9755d-102">لا تظهر تسميات الحساسية</span><span class="sxs-lookup"><span data-stu-id="9755d-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="9755d-103">تسمح لك تسميات الحساسية بتصنيف المحتوي الحساس والمساعدة في حمايته.</span><span class="sxs-lookup"><span data-stu-id="9755d-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="9755d-104">يمكن إنشائها في مركز التوافق ل Microsoft 365 أو مركز الأمان ل microsoft 365 أو Microsoft 365 security & مركز التوافق ضمن تصنيف > الحساسية.</span><span class="sxs-lookup"><span data-stu-id="9755d-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="9755d-105">لمعرفه المزيد حول هذه الميزة ، راجع [نظره عامه حول تسميات الحساسية](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="9755d-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels).</span></span>

<span data-ttu-id="9755d-106">إذا قمت بتكوين تسميات الحساسية الخاصة بك ولكنها لا تظهر في تطبيقات Microsoft 365 ، فتحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="9755d-106">If you configured your sensitivity labels but they aren't appearing in the Microsoft 365 apps, check the following:</span></span>

- <span data-ttu-id="9755d-107">تاكد من انه تم [نشر](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) تسميه الحساسية إلى المستخدمين والمجموعات التي تريدها.</span><span class="sxs-lookup"><span data-stu-id="9755d-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="9755d-108">تاكد من ان المستخدم يستخدم تطبيقا يعتمد تسميات الحساسية-راجع [تسميات الحساسية في المستند](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="9755d-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="9755d-109">إذا كنت تقوم [بترحيل تسميات حماية البيانات في Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)، فيجب ان تكون علي علم بالاعتبارات المذكورة [هنا](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="9755d-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="9755d-110">دعم منع فقدان البيانات (DLP): يمكن استخدام تسميات الاستبقاء حاليا كشرط في نهج DLP.</span><span class="sxs-lookup"><span data-stu-id="9755d-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="9755d-111">لا يتوفر دعم لتسميات الحساسية في نهج DLP حتى الآن ولكننا نعمل علي ذلك.</span><span class="sxs-lookup"><span data-stu-id="9755d-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="9755d-112">عند تمكين التشفير في تسميه الحساسية ، يمكنك الاختيار اما إلى:</span><span class="sxs-lookup"><span data-stu-id="9755d-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="9755d-113">تعيين الأذونات الآن</span><span class="sxs-lookup"><span data-stu-id="9755d-113">Assign permissions now</span></span>
    - <span data-ttu-id="9755d-114">السماح للمستخدمين بتعيين الأذونات</span><span class="sxs-lookup"><span data-stu-id="9755d-114">Let users assign permissions</span></span>


<span data-ttu-id="9755d-115">لمزيد من المعلومات حول المشاكل المحتملة ، راجع [المشاكل المعروفة باستخدام تسميات الحساسية](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="9755d-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>