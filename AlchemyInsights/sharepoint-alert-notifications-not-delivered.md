---
title: لم يتم تسليم اعلامات التنبيه في SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: f4002dc865fb7a03b07a9256709b947d6d774cb0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751230"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a><span data-ttu-id="314a9-102">لم يتم تسليم اعلامات التنبيه في SharePoint</span><span class="sxs-lookup"><span data-stu-id="314a9-102">SharePoint alert notifications not delivered</span></span>

<span data-ttu-id="314a9-103">يرجى التحقق من مجلد البريد الكتروني غير الهام ، وقد ينتقل التنبيات أحيانا.</span><span class="sxs-lookup"><span data-stu-id="314a9-103">Please check the JUNK folder in your email, as sometimes alerts might go there.</span></span>

<span data-ttu-id="314a9-104">تحديد ما إذا كانت **كل التنبيات لا يتم تسليمها** أو إذا لم يتم تسليم **تنبيه فردي** من ملف أو مكتبه معينه.</span><span class="sxs-lookup"><span data-stu-id="314a9-104">Determine if **all alerts are not delivered** or if **an individual alert** from a specific file or library is not delivered.</span></span>

- <span data-ttu-id="314a9-105">**لا يتم تسليم التنبيات الفردية**: إذا لم يتم تسليم تنبيه فردي من ملف أو مكتبه معينه ، فيمكنك محاولة حذفه وأعاده إنشائه.</span><span class="sxs-lookup"><span data-stu-id="314a9-105">**Individual alerts are not delivered**: If an individual alert from a specific file or library is not delivered, you can attempt to delete and recreate it.</span></span> <span data-ttu-id="314a9-106">راجع [أداره تنبيات SharePoint أو عرضها أو حذفها](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) لأعاده إنشاء التنبيه.</span><span class="sxs-lookup"><span data-stu-id="314a9-106">See [Manage, view, or delete SharePoint alerts](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>
- <span data-ttu-id="314a9-107">**لا يتم تسليم كل التنبيات**: إذا لم يتم تسليم كل التنبيات من ملفات أو مكتبات متعددة ، فيمكنك زيارة [لوحه معلومات حماية الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) للتحقق من اي نصائح/حوادث قد تحدث في SharePoint أو Exchange.</span><span class="sxs-lookup"><span data-stu-id="314a9-107">**All alerts are not delivered**: If all alerts from multiple files or libraries are not delivered, visit the [Service Health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="314a9-108">قد تكون المشكلة باستخدام امكانيه تنبيه SharePoint أو التاخيرات في رسائل البريد الكتروني من خلال Exchange.</span><span class="sxs-lookup"><span data-stu-id="314a9-108">The issue could be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="314a9-109">سيكون من المهم ملاحظه ما إذا كان يتم تسليم البريد الكتروني الآخر ، وما إذا كان الأمر كذلك ، فمن المحتمل ان تكون المشكلة في حاله حدوث تاخيرات في Exchange.</span><span class="sxs-lookup"><span data-stu-id="314a9-109">It will also be important to note whether other email is being delivered, and if not, the issue is likely with Exchange delays.</span></span>

<span data-ttu-id="314a9-110">الاسئله المتداولة حول التنبيات:</span><span class="sxs-lookup"><span data-stu-id="314a9-110">FAQ on alerts:</span></span>

- <span data-ttu-id="314a9-111">لا يمكن إرسال التنبيات إلى مجموعه التوزيع ، ولا يتم دعم سوي مجموعات الأمان و O365.</span><span class="sxs-lookup"><span data-stu-id="314a9-111">It is not possible to send alerts to Distribution Group, only Security and O365 groups are supported.</span></span>
- <span data-ttu-id="314a9-112">لا يمكنك تخصيص قوالب التنبيات عبر البريد الكتروني ؛ أنت بحاجه إلى استخدام سير عمل Microsoft تدفق أو SharePoint Designer للوصول إلى العناصر التالية.</span><span class="sxs-lookup"><span data-stu-id="314a9-112">You cannot customize alert email templates; you need to use Microsoft FLOW or SharePoint Designer Workflow to achieve those.</span></span>

## <a name="related-topics"></a><span data-ttu-id="314a9-113">مواضيع ذات صله</span><span class="sxs-lookup"><span data-stu-id="314a9-113">Related Topics</span></span>

<span data-ttu-id="314a9-114">هل تريد تجربه Microsoft تدفق في SharePoint Online ؟</span><span class="sxs-lookup"><span data-stu-id="314a9-114">Want to try Microsoft Flow in SharePoint Online?</span></span>

- [<span data-ttu-id="314a9-115">إنشاء تدفق</span><span class="sxs-lookup"><span data-stu-id="314a9-115">Create Flow</span></span>](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [<span data-ttu-id="314a9-116">SharePoint والتدفق</span><span class="sxs-lookup"><span data-stu-id="314a9-116">SharePoint and Flow</span></span>](https://flow.microsoft.com//blog/sharepoint-and-flow/)
