---
title: نقل رسائل البريد الإلكتروني تلقائيا إلى علبة بريد الأرشيف
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523347"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a><span data-ttu-id="61859-102">نقل رسائل البريد الإلكتروني تلقائيا إلى علبة بريد الأرشيف</span><span class="sxs-lookup"><span data-stu-id="61859-102">Automatically move email messages to the archive mailbox</span></span>

<span data-ttu-id="61859-103">فيما يلي كيفية إعداد نهج لنقل البريد الإلكتروني القديم الخاص بالمستخدم تلقائيا إلى علبة بريد الأرشيف:</span><span class="sxs-lookup"><span data-stu-id="61859-103">Here's how to set up a policy to automatically move a user's old email to the archive mailbox:</span></span>

1. <span data-ttu-id="61859-104">انتقل إلى [**"الأمان& "أرشيف**](https://go.microsoft.com/fwlink/p/?linkid=2077143)إدارة بيانات التوافق" للتحقق من تمكين علبة بريد الأرشيف  >    >   للمستخدم.</span><span class="sxs-lookup"><span data-stu-id="61859-104">Go to [**Security & Compliance**](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **Data governance** > **Archive** to verify an archive mailbox has been enabled for the user.</span></span> <span data-ttu-id="61859-105">إذا لم يحدث ذلك، انقر **فوق** "تمكين" ثم **"نعم"** في مربع التحذير.</span><span class="sxs-lookup"><span data-stu-id="61859-105">If it hasn't, click **Enable** then **Yes** in the warning box.</span></span>
2. <span data-ttu-id="61859-106">انتقل إلى [**مركز إدارة Exchange > إدارة > علامات الاستبقاء.**](https://go.microsoft.com/fwlink/?linkid=2059104)</span><span class="sxs-lookup"><span data-stu-id="61859-106">Go to [**Exchange admin center > compliance management > retention tags**](https://go.microsoft.com/fwlink/?linkid=2059104).</span></span>
3. <span data-ttu-id="61859-107">اختر الأيقونة + ثم **اختر تطبيق التطبيق تلقائيا على علبة البريد بأكملها.**</span><span class="sxs-lookup"><span data-stu-id="61859-107">Choose the + icon then choose **automatically apply to entire mailbox**.</span></span>
4. <span data-ttu-id="61859-108">قم بتعيين اسم لعلامة الاستبقاء، واختر **"نقل إلى الأرشيف".**</span><span class="sxs-lookup"><span data-stu-id="61859-108">Assign a name to the retention tag, and choose **Move to Archive**.</span></span> <span data-ttu-id="61859-109">بالنسبة إلى فترة الاستبقاء، أدخل الوقت الذي تريده، مثل 90 يوما.</span><span class="sxs-lookup"><span data-stu-id="61859-109">For the retention period, enter the time you want, such as 90 days.</span></span> <span data-ttu-id="61859-110">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="61859-110">Click **Save**.</span></span>
5. <span data-ttu-id="61859-111">أنشئ الآن نهج استبقاء: اختر **نهج الاستبقاء،** واختر الأيقونة لإضافة نهج جديد.</span><span class="sxs-lookup"><span data-stu-id="61859-111">Now create a retention policy: choose **retention policies**, choose the icon to add a new policy.</span></span>
6. <span data-ttu-id="61859-112">قم بتعيين اسم إلى نهج الاستبقاء، ثم انقر ثم قم بالتمرير للعثور على علامة الاستبقاء التي أنشأتها للتو وإضافتها.</span><span class="sxs-lookup"><span data-stu-id="61859-112">Assign a name to the retention policy, then click and scroll to find and add the retention tag you just created.</span></span> <span data-ttu-id="61859-113">انقر فوق **حفظ**.</span><span class="sxs-lookup"><span data-stu-id="61859-113">Click **Save**.</span></span>
7. <span data-ttu-id="61859-114">وأخيرا، طبق نهج الاستبقاء على علبة بريد المستخدم: في مركز إدارة Exchange، انتقل إلى **علب** بريد  >  **المستلمين.**</span><span class="sxs-lookup"><span data-stu-id="61859-114">Finally, apply the retention policy to the user's mailbox: still in the Exchange admin center, go to **recipients** > **mailboxes**.</span></span> <span data-ttu-id="61859-115">اختر جميع المستخدمين الذين تريد تطبيق النهج لديهم، ثم اختر **"تحرير"** (أيقونة القلم الرصاص).</span><span class="sxs-lookup"><span data-stu-id="61859-115">Choose all the users who you want to apply the policy to, then choose **Edit** (the pencil icon).</span></span>
8. <span data-ttu-id="61859-116">في مربع الحوار، انقر فوق ميزات **علبة البريد.**</span><span class="sxs-lookup"><span data-stu-id="61859-116">In the dialog box, click **mailbox features**.</span></span> <span data-ttu-id="61859-117">ضمن **نهج الاستبقاء،** طبق النهج الذي أنشأته للتو > **حفظ.**</span><span class="sxs-lookup"><span data-stu-id="61859-117">Under **Retention policy**, apply the policy you just created > **Save**.</span></span>
9. <span data-ttu-id="61859-118">للحصول على إرشادات حول تطبيق النهج على جميع المستخدمين، راجع [تطبيق نهج استبقاء على علب البريد.](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)</span><span class="sxs-lookup"><span data-stu-id="61859-118">For instructions for applying the policy to all users, see [Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).</span></span>
