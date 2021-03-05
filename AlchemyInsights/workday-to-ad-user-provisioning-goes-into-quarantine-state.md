---
title: يوم عمل لتوفير مستخدم AD إلى حالة الفحص
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/04/2021
ms.locfileid: "50480839"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="ded88-102">يوم عمل لتوفير مستخدم AD إلى حالة الفحص</span><span class="sxs-lookup"><span data-stu-id="ded88-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="ded88-103">**يوم عمل لتوفير مستخدم AD إلى حالة الفحص ولا يتم إنشاء أي مستخدمين في AD**</span><span class="sxs-lookup"><span data-stu-id="ded88-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="ded88-104">لقد وصلت مهمة توفير يوم العمل لمستخدم AD إلى حالة الفحص وتظهر سجلات التدقيق أحداث فشل التصدير مع رسالة **الخطأ: OperationsError-SvcErr: حدث خطأ في العملية. لم يتم تكوين مرجع أفضل لخدمة الدليل. وبالتالي، يتعذر** على خدمة الدليل إصدار إحالات إلى كائنات خارج هذه الغابات.</span><span class="sxs-lookup"><span data-stu-id="ded88-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="ded88-105">يظهر هذا الخطأ عادة إذا لم يتم تعيين OU حاوية Active Directory بشكل صحيح أو إذا كانت هناك مشاكل في تعيين التعبير المستخدم ل **parentDistinguishedName.**</span><span class="sxs-lookup"><span data-stu-id="ded88-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="ded88-106">تحقق من معلمة OU الافتراضية **للمستخدمين** الجدد للتأكد من الأخطاء الطباعية.</span><span class="sxs-lookup"><span data-stu-id="ded88-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="ded88-107">تأكد من وجود OU المحدد بالفعل في AD.</span><span class="sxs-lookup"><span data-stu-id="ded88-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="ded88-108">إذا كنت تستخدم **parentDistinguishedName** في تعيين السمة، فتأكد من تقييمها دائما إلى حاوية معروفة داخل مجال AD.</span><span class="sxs-lookup"><span data-stu-id="ded88-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="ded88-109">تحقق من الحدث "تصدير" في سجلات التدقيق لرؤية القيمة التي تم إنشاؤها.</span><span class="sxs-lookup"><span data-stu-id="ded88-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="ded88-110">لمزيد من التفاصيل حول تكوين يوم العمل للتكوين التلقائي، راجع البرنامج [التعليمي: تكوين يوم](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)عمل للتكوين التلقائي للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="ded88-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

