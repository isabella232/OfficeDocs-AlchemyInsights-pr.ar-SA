---
title: تعليقات علي عناصر القائمة
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
- "9003821"
- "6841"
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982417"
---
# <a name="comments-on-list-items"></a><span data-ttu-id="46ebf-102">تعليقات علي عناصر القائمة</span><span class="sxs-lookup"><span data-stu-id="46ebf-102">Comments on List items</span></span>

<span data-ttu-id="46ebf-103">سيتمكن المستخدمون قريبا من أضافه التعليقات وحذفها من عناصر القائمة.</span><span class="sxs-lookup"><span data-stu-id="46ebf-103">Users will soon be able to add and delete comments on list items.</span></span> <span data-ttu-id="46ebf-104">يمكن للمستخدمين عرض كل التعليقات علي عنصر قائمه وتصفيه بين طرق العرض التي تعرض التعليقات أو النشاط المرتبط بعنصر.</span><span class="sxs-lookup"><span data-stu-id="46ebf-104">Users can view all comments on a list item and filter between views that show comments or activity related to an item.</span></span>

<span data-ttu-id="46ebf-105">**التوقيت** :</span><span class="sxs-lookup"><span data-stu-id="46ebf-105">**Timing** :</span></span>

<span data-ttu-id="46ebf-106">**الإصدار المستهدف** : التعبئة التدريجية في منتصف الاكتوبر والمتوقع إكمالها بواسطة المتوسط-نوفمبر</span><span class="sxs-lookup"><span data-stu-id="46ebf-106">**Targeted release** : Gradual roll out in mid-October and expected to complete by mid-November</span></span>

<span data-ttu-id="46ebf-107">**الإصدار القياسي** : التعبئة التدريجية في منتصف النوفمبر والمتوقع إكمالها في وقت ديسمبر المبكر</span><span class="sxs-lookup"><span data-stu-id="46ebf-107">**Standard release** : Gradual roll out in mid-November and expected to complete by early December</span></span>

<span data-ttu-id="46ebf-108">العمليات **التمهيدية** : الإصدار المستهدف للمؤسسة بأكملها</span><span class="sxs-lookup"><span data-stu-id="46ebf-108">**Rollout** : Targeted release for the entire organization</span></span>

<span data-ttu-id="46ebf-109">يجب علي المستخدمين ملاحظه ما يلي قبل ان يتمكنوا من أضافه التعليقات وحذفها:</span><span class="sxs-lookup"><span data-stu-id="46ebf-109">Users need to note the following before they can add and delete comments:</span></span>

- <span data-ttu-id="46ebf-110">تتبع التعليقات إعدادات الأذونات المضمنة في SharePoint.</span><span class="sxs-lookup"><span data-stu-id="46ebf-110">Comments follow the permission settings inherent in SharePoint.</span></span>
- <span data-ttu-id="46ebf-111">القوائم الكلاسيكية التي لم يتم إنشاؤها بعد لتظهر في واجات المستخدم الحديثة ، مثل قوائم المهام ، لن تتوفر لميزه التعليق هذه.</span><span class="sxs-lookup"><span data-stu-id="46ebf-111">Classic lists that are not yet built to show up in modern user interfaces, like task lists, will not have this commenting feature.</span></span>
- <span data-ttu-id="46ebf-112">لا تتوفر التعليقات علي القوائم في الفرق مع هذا الإصدار.</span><span class="sxs-lookup"><span data-stu-id="46ebf-112">Commenting on lists in Teams is not available with this release.</span></span>
- <span data-ttu-id="46ebf-113">التعليقات غير مفهرسه بالبحث.</span><span class="sxs-lookup"><span data-stu-id="46ebf-113">Comments are not indexed by Search.</span></span>

<span data-ttu-id="46ebf-114">يمكن للمسؤولين تعطيل هذه الميزة علي مستوي المؤسسة بتغيير المعلمة **كوممينتسونليستيتيمسديسابليد** في **المجموعة سبوتينانت** PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="46ebf-114">Admins can disable this feature at the organization level by changing the **CommentsOnListItemsDisabled** parameter in the **Set-SPOTenant** PowerShell cmdlet.</span></span>

<span data-ttu-id="46ebf-115">لا يمكن حاليا تعطيل التعليق علي مستوي الموقع أو القائمة.</span><span class="sxs-lookup"><span data-stu-id="46ebf-115">It is not currently possible to disable commenting at the site or list level.</span></span> <span data-ttu-id="46ebf-116">نامل ان يكون لديك عناصر التحكم هذه في تحديث لاحق ، علي الأرجح في أول ربع سنه 2021.</span><span class="sxs-lookup"><span data-stu-id="46ebf-116">We hope to have those controls in a later update, likely in the first quarter 2021.</span></span>
