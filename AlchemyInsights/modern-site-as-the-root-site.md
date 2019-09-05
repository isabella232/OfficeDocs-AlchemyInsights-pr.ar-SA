---
title: الموقع الحديث كموقع الجذر
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: a3cf44d52a3948634fc0eed64c852ff17515fd9b
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753891"
---
# <a name="modern-site-as-root-site"></a>الموقع الحديث كموقع جذر

لقد بدأنا في طرح ميزة جديدة من شأنها أن تسمح لك [لمبادلة موقعك الجذر الكلاسيكية مع موقع حديث.](https://docs.microsoft.com/sharepoint/modern-root-site) استخدم [استدعاء SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادلة موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.

>[!Important]
> لا تقم بحذف موقع الجذر الكلاسيكي لإنشاء موقع اتصال حديث. هذا غير معتمد من قبل Microsoft. سيؤدي حذف الموقع الجذر إلى جعل كافة مواقع SharePoint في مؤسستك غير قابلة للوصول إلى كافة المستخدمين، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في نفس محدد موقع المعلومات .( سنقوم بتوصيل هذه الميزة عبر مركز الرسائل. يجب أن تتوقع الميزة ليتم تشغيلها في المستأجر الخاص بك قريباً.

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع مواقع المبادلة
- قد يرجع الموقع الهدف خطأ "لم يتم العثور عليها" (HTTP 404) لفترة قصيرة من الوقت.
- يجب إعادة تتبع ارتباطات المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة هنا، وسيتم ذلك تلقائيا.
- يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملف وملفات OneNote) يدويًا.
- قد تحتاج مواقع خادم Project إلى التحقق من صحة للتأكد من أنها لا تزال مقترنة بشكل صحيح. 
