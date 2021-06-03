---
title: شحن محرك الأقراص في Microsoft 365 الاستيراد
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731254"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="bfb5b-102">شحن محرك الأقراص في Microsoft 365 الاستيراد</span><span class="sxs-lookup"><span data-stu-id="bfb5b-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="bfb5b-103">استخدم شحن محرك الأقراص عن طريق نسخ PSTs إلى محرك أقراص صلبة ثم شحن محرك الأقراص الثابت إلى Microsoft.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="bfb5b-104">لبدء المهمة:</span><span class="sxs-lookup"><span data-stu-id="bfb5b-104">To start the job:</span></span>

1. <span data-ttu-id="bfb5b-105">في مركز Microsoft 365 ضمن **إدارة المعلومات،** حدد **استيراد**.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="bfb5b-106">حدد **اختيار نوع مهمة الاستيراد**، ثم حدد **التالي**.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="bfb5b-107">لرؤية الخطوات الخاصة بخيار الاستيراد هذا، حدد شحن محركات الأقراص الثابت **إلى أحد مواقعنا الفعلية**.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="bfb5b-108">فيما يلي بعض الأمور التي يجب تذكرها:</span><span class="sxs-lookup"><span data-stu-id="bfb5b-108">Here are some things to remember:</span></span>

- <span data-ttu-id="bfb5b-109">يجب أن يتم تعيين دور استيراد تصدير علب البريد في Exchange Online استيراد ملفات PST Microsoft 365 علب البريد.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="bfb5b-110">قد يؤثر الأداء على PSTs التي يزيد حجمها عن 20 غيغابايت.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="bfb5b-111">محركات الأقراص ذات الحالة الصلبة (SSDs) بحجم 2.5 بوصة فقط أو محركات الأقراص الثابت الداخلية SATA II/III بحجم 2.5 بوصة أو 3.5 بوصة معتمدة.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="bfb5b-112">يجب تشفير محرك الأقراص الثابت الذي يحتوي على ملفات PST باستخدام BitLocker.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="bfb5b-113">تبلغ تكلفة استيراد ملفات PST Microsoft 365 علب البريد باستخدام شحن محرك الأقراص 2 دولار أمريكي لكل غيغابايت من البيانات.</span><span class="sxs-lookup"><span data-stu-id="bfb5b-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="bfb5b-114">للحصول على معلومات إضافية حول استخدام طريقة شحن محرك الأقراص لاستيراد PSTs، راجع استخدام شحن محرك الأقراص لاستيراد ملفات [PST الخاصة مؤسستك.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="bfb5b-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>