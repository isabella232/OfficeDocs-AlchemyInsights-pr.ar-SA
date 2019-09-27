---
title: تسميات الحساسية لا تظهر
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 4bf8e02246c966f22648467386a7862f0521fecf
ms.sourcegitcommit: 71978e2bb779b5955fd113f84512b83321b26912
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/26/2019
ms.locfileid: "37207212"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="f9975-102">تسميات الحساسية لا تظهر</span><span class="sxs-lookup"><span data-stu-id="f9975-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="f9975-103">تسمح لك تسميات الحساسية بتصنيف المحتوي الحساس والمساعدة علي حمايته.</span><span class="sxs-lookup"><span data-stu-id="f9975-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="f9975-104">يمكن إنشاؤها في مركز التوافق Microsoft 365 أو مركز أمان Microsoft 365 أو Office 365 الأمان & مركز التوافق ضمن تصنيف > الحساسية التسميات.</span><span class="sxs-lookup"><span data-stu-id="f9975-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Office 365 Security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="f9975-105">لمعرفه المزيد حول هذه الميزة ، راجع [نظره عامه علي تسميات الحساسية](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span><span class="sxs-lookup"><span data-stu-id="f9975-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="f9975-106">إذا قمت بتكوين تسميات الحساسية الخاصة بك ولكنها لا تظهر في تطبيقات Office ، فتحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="f9975-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="f9975-107">تاكد من ان تسميه الحساسية قد تم [نشرها](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) إلى المستخدمين والمجموعات التي تريدها.</span><span class="sxs-lookup"><span data-stu-id="f9975-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="f9975-108">تاكد من ان المستخدم يستخدم تطبيقا يدعم تسميات الحساسية-راجع [تسميات الحساسية في المستند](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span><span class="sxs-lookup"><span data-stu-id="f9975-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="f9975-109">إذا كنت تقوم [بترحيل تسميات حماية معلومات Azure](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)، يجب ان تكون علي علم بالاعتبارات المسرودة [هنا](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span><span class="sxs-lookup"><span data-stu-id="f9975-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="f9975-110">دعم منع فقدان البيانات (DLP): حاليا ، يمكن استخدام تسميات الاستبقاء فقط كشرط في نهج DLP.</span><span class="sxs-lookup"><span data-stu-id="f9975-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="f9975-111">دعم التسميات حساسية في سياسة DLP غير متوفرة حتى الآن ولكن نحن نعمل علي ذلك.</span><span class="sxs-lookup"><span data-stu-id="f9975-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="f9975-112">عند تمكين التشفير علي تسميه تحسسيه ، يمكنك اختيار اما:</span><span class="sxs-lookup"><span data-stu-id="f9975-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="f9975-113">تعيين الأذونات الآن</span><span class="sxs-lookup"><span data-stu-id="f9975-113">Assign permissions now</span></span>
    - <span data-ttu-id="f9975-114">السماح للمستخدمين بتعيين أذونات</span><span class="sxs-lookup"><span data-stu-id="f9975-114">Let users assign permissions</span></span>


<span data-ttu-id="f9975-115">لمزيد من المعلومات حول المشكلات المحتملة ، راجع [المشكلات المعروفة مع تسميات الحساسية](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span><span class="sxs-lookup"><span data-stu-id="f9975-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>