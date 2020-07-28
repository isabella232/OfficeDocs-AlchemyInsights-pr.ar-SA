---
title: لم يتم إعداد Apple MDM Certificate
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/28/2020
ms.locfileid: "45438699"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="3fa45-102">لم يتم إعداد Apple MDM Certificate</span><span class="sxs-lookup"><span data-stu-id="3fa45-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="3fa45-103">لم يتم تكوين شهادة دفع Apple MDM (المعروفة أيضًا باسم شهادة خدمة الإعلامات المقدمة من Apple (APNS) للاشتراك.</span><span class="sxs-lookup"><span data-stu-id="3fa45-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="3fa45-104">بدون تكوين شهادة دفع من Apple MDM، لن تتمكن من تسجيل أجهزة iOS و Mac OS وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="3fa45-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="3fa45-105">بعد إضافة الشهادة إلى Intune، يمكن للمستخدمين تثبيت تطبيق Company Portal لتسجيل أجهزة iOS الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="3fa45-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="3fa45-106">حدد **"أوافق".**</span><span class="sxs-lookup"><span data-stu-id="3fa45-106">Select **"I agree."**</span></span> <span data-ttu-id="3fa45-107">لإعطاء Microsoft الإذن لإرسال البيانات إلى Apple.</span><span class="sxs-lookup"><span data-stu-id="3fa45-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="3fa45-108">حدد **تنزيل CSR** طلب توقيع شهادة Intune المطلوب لإنشاء شهادة دفع Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="3fa45-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="3fa45-109">يتم استخدام الملف لطلب شهادة علاقة ثقة من "مدخل شهادات الدفع أبل".</span><span class="sxs-lookup"><span data-stu-id="3fa45-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="3fa45-110">حدد **إنشاء شهادة دفع MDM** للانتقال إلى مدخل شهادات الدفع التفاح.</span><span class="sxs-lookup"><span data-stu-id="3fa45-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="3fa45-111">سجّل الدخول باستخدام Apple ID للشركة، ثم حدد **إنشاء شهادة**.</span><span class="sxs-lookup"><span data-stu-id="3fa45-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="3fa45-112">حدد **اختيار ملف**، واستعرض إلى ملف طلب توقيع الشهادة، ثم اختر **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="3fa45-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="3fa45-113">في صفحة التأكيد، اختر **تنزيل** لتنزيل ملف الشهادة (.pem)، ثم احفظ الملف محلياً.</span><span class="sxs-lookup"><span data-stu-id="3fa45-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="3fa45-114">**ملاحظة:** ترتبط الشهادة بمعرف Apple ID المستخدم في إنشائها.</span><span class="sxs-lookup"><span data-stu-id="3fa45-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="3fa45-115">وكأفضل ممارسة، استخدم Apple ID الشركة لمهام الإدارة، وتأكد من مراقبة صندوق البريد من قبل أكثر من شخص واحد أو باستخدام قائمة توزيع.</span><span class="sxs-lookup"><span data-stu-id="3fa45-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="3fa45-116">لا تستخدم أبدًا Apple ID شخصيًا.</span><span class="sxs-lookup"><span data-stu-id="3fa45-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="3fa45-117">استخدم نفس Apple ID لتجديد شهادة Apple Push كل 12 شهرًا.</span><span class="sxs-lookup"><span data-stu-id="3fa45-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="3fa45-118">أدخل Apple ID المستخدم لإنشاء شهادة الدفع من Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="3fa45-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="3fa45-119">سجل هذا المعرف كتذكير عندما تحتاج إلى تجديد الشهادة.</span><span class="sxs-lookup"><span data-stu-id="3fa45-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="3fa45-120">انتقل إلى ملف الشهادة (.pem) واختر **فتح**، ثم اختر **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="3fa45-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="3fa45-121">مع شهادة الدفع ، يمكن لـ Intune تسجيل أجهزة Apple وإدارتها.</span><span class="sxs-lookup"><span data-stu-id="3fa45-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>