---
title: إضافة توقيع شركة عام أو إخلاء المسؤولية لجميع المستخدمين
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
ms.openlocfilehash: ab0d3fc80b41b9017a6917817270438644f770b8
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/05/2021
ms.locfileid: "50480953"
---
# <a name="add-a-global-company-signature-or-disclaimer-for-all-users"></a><span data-ttu-id="b2b6e-102">إضافة توقيع شركة عام أو إخلاء المسؤولية لجميع المستخدمين</span><span class="sxs-lookup"><span data-stu-id="b2b6e-102">Add a global company signature or disclaimer for all users</span></span>

<span data-ttu-id="b2b6e-103">تلميح: يسمى التوقيع على مستوى المؤسسة أيضا إخلاء المسؤولية، بغض النظر عما يتضمنه.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-103">Tip: An org-wide signature is also called a disclaimer, regardless of what it includes.</span></span>

1. <span data-ttu-id="b2b6e-104">في مركز الإدارة، اختر **مراكز**  >  **الإدارة Exchange.**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-104">In the admin center, choose **Admin centers** > **Exchange**.</span></span>
2. <span data-ttu-id="b2b6e-105">ضمن تدفق البريد، اختر **"القواعد".**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-105">Under Mail flow, choose **Rules**.</span></span>
3. <span data-ttu-id="b2b6e-106">انقر فوق **+** الأيقونة (إضافة) واختر **تطبيق إخلاء المسؤولية.**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-106">Click the **+** (Add) icon and choose **Apply disclaimers**.</span></span>
4. <span data-ttu-id="b2b6e-107">امنح القاعدة اسما.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-107">Give the rule a name.</span></span>
5. <span data-ttu-id="b2b6e-108">ضمن "تطبيق هذه القاعدة"، اختر **"تطبيق على كل الرسائل".**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-108">Under Apply this rule, choose **Apply to all messages**.</span></span>
6. <span data-ttu-id="b2b6e-109">ضمن "القيام بما يلي"، اترك **"إلحاق** بيان إخلاء المسؤولية" محددا.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-109">Under Do the following, leave **Append the disclaimer** selected.</span></span>
7. <span data-ttu-id="b2b6e-110">انقر **فوق إدخال نص** وادخل بيان إخلاء المسؤولية.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-110">Click **Enter text** and type your disclaimer.</span></span>
8. <span data-ttu-id="b2b6e-111">انقر **فوق "تحديد واحد"،** **واختر** "التفاف" كخيار خلفي، ثم انقر فوق **"موافق".**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-111">Click **Select one**, choose **Wrap** as a fallback option, and then click **OK**.</span></span> <span data-ttu-id="b2b6e-112">وهذا يعني أنه إذا لم يكن من الممكن إضافة بيان إخلاء المسؤولية بسبب التشفير أو إعداد بريد آخر، سيتم التفافه في مغلف رسالة.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-112">This means that if the disclaimer can't be added because of encryption or another mail setting, it will be wrapped in a message envelope.</span></span>
9. <span data-ttu-id="b2b6e-113">اترك **"تدقيق" هذه القاعدة** مع تحديد مستوى الخطورة.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-113">Leave **Audit this rule** with severity level selected.</span></span> <span data-ttu-id="b2b6e-114">ثم اختر "منخفض" أو "متوسط" أو "عال" لتستخدمه في سجل الرسائل.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-114">Then choose Low, Medium, or High to be used in the message log.</span></span>
10. <span data-ttu-id="b2b6e-115">اختر **"فرض"** لقلب بيان إخلاء المسؤولية على الفور، إلا إذا كنت تريد اختباره أولا.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-115">Choose **Enforce** to turn on the disclaimer immediately, unless you want to test it first.</span></span>
11. <span data-ttu-id="b2b6e-116">اختر **المزيد من الخيارات** لتضمين شروط أو استثناءات إضافية.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-116">Choose **More options** to include additional conditions or exceptions.</span></span>
12. <span data-ttu-id="b2b6e-117">عند الانتهاء، انقر فوق **"حفظ".**</span><span class="sxs-lookup"><span data-stu-id="b2b6e-117">When finished, click **Save**.</span></span>
13. <span data-ttu-id="b2b6e-118">هل تحتاج إلى مزيد من المساعدة؟</span><span class="sxs-lookup"><span data-stu-id="b2b6e-118">Need more help?</span></span> [<span data-ttu-id="b2b6e-119">شاهد فيديو حول إنشاء إخلاء المسؤولية أو اقرأ المقالة بالكامل.</span><span class="sxs-lookup"><span data-stu-id="b2b6e-119">Watch a video about creating disclaimers or read the full article.</span></span>](https://support.office.com/article/2d75860f-c527-4352-a7f6-73eba54c0c72?wt.mc_id=Chat_GlobalSignature)