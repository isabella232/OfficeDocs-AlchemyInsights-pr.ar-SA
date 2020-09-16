---
title: لم يتم اعداد شهادة الدفع في Apple MDM
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716844"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="fa0f6-102">لم يتم اعداد شهادة الدفع في Apple MDM</span><span class="sxs-lookup"><span data-stu-id="fa0f6-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="fa0f6-103">لم يتم تكوين شهادة الدفع الخاصة ب Apple MDM (المعروفة أيضا بشهادة خدمه الاعلام بالإرسال إلى Apple (APNS)) لاشتراكك.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="fa0f6-104">بدون تكوين شهادة Apple MDM ، لا يمكنك تسجيل أجهزه iOS و Mac OS وأدارتها.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="fa0f6-105">بعد أضافه الشهادة إلى Intune ، يمكن للمستخدمين تثبيت تطبيق مدخل الشركة لتسجيل أجهزه iOS الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="fa0f6-106">حدد **"أوافق."**</span><span class="sxs-lookup"><span data-stu-id="fa0f6-106">Select **"I agree."**</span></span> <span data-ttu-id="fa0f6-107">لمنح Microsoft الاذن بإرسال البيانات إلى Apple.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="fa0f6-108">حدد تنزيل "المطالبة بتسجيل الدخول إلى الترخيص في Intune" لإنشاء شهادة الدفع **الخاصة** ب Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="fa0f6-109">يتم استخدام الملف لطلب شهادة علاقة ثقة من مدخل الشهادات الخاصة ب Apple.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="fa0f6-110">حدد **إنشاء شهادة الدفع MDM** للانتقال إلى مدخل شهادات الدفع في Apple.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="fa0f6-111">قم بتسجيل الدخول باستخدام معرف Apple الخاص بشركك ، ثم حدد **إنشاء شهادة**.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="fa0f6-112">حدد **اختيار ملف**، واستعرض وصولا إلى ملف طلب توقيع الشهادة ، ثم اختر **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="fa0f6-113">في صفحه التاكيد ، اختر **تنزيل** لتنزيل ملف الشهادة (pem) ، واحفظ الملف محليا.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="fa0f6-114">**ملاحظه**: تقترن الشهادة بمعرف Apple المستخدم لإنشاءها.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="fa0f6-115">كافضل ممارسه ، استخدم معرف Apple الخاص بالشركة لمهام الاداره ، وتاكد من انه تمت مراقبه علبه البريد بواسطة أكثر من شخص واحد أو باستخدام قائمه توزيع.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="fa0f6-116">لا تستخدم أبدا معرف Apple الشخصي.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="fa0f6-117">استخدم معرف Apple نفسه لتجديد شهادة دفع Apple كل 12 شهرا.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="fa0f6-118">ادخل معرف Apple المستخدم لإنشاء شهادة الدفع الخاصة ب Apple MDM.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="fa0f6-119">سجل هذا المعرف كتذكير عندما تحتاج إلى تجديد الشهادة.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="fa0f6-120">انتقل إلى ملف الشهادة (pem) ، واختر **فتح**، ثم اختر **تحميل**.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="fa0f6-121">باستخدام شهادة الدفع ، يمكن ل Intune تسجيل أجهزه Apple وأدارتها.</span><span class="sxs-lookup"><span data-stu-id="fa0f6-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>