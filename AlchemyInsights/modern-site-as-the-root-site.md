---
title: الموقع الحديث ك الموقع الجذر
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: b42cf276a76547584c8cfd87b5a28f31d51ea7f8ca56621b22aeef01e4613ce6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000373"
---
# <a name="modern-site-as-root-site"></a>الموقع الحديث كم موقع الجذر

لقد بدأنا في طرح ميزة جديدة تسمح لك بتبادلة موقع الجذر الكلاسيكي الخاص بك [مع موقع حديث](https://docs.microsoft.com/sharepoint/modern-root-site). استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع بموقع آخر أثناء أرشفة الموقع الأصلي. يتوفر لكل من موقع الفريق (غير متصل بمجموعة) و"موقع الاتصالات".

>[!Important]
> لا تحذف موقعك الجذر الكلاسيكي لإنشاء موقع اتصالات حديث. لا تدعم Microsoft هذا الأمر. سيتعذر على جميع المستخدمين حذف الموقع الجذر الوصول إلى كل SharePoint في مؤسستك، إلى أن تستعيد الموقع أو تنشئ موقعا جديدا في عنوان URL نفسه. سنقوم بتواصل هذه الميزة عبر مركز الرسائل. يجب أن تتوقع تشغيل الميزة في المستأجر الخاص بك قريبا.

## <a name="known-issues-with-swapping-sites"></a>المشاكل المعروفة في تبديل المواقع
- قد يرجع الموقع الهدف الخطأ "لم يتم العثور عليه" (HTTP 404) لفترة زمنية قصيرة.
- يجب إعادة فهرسة المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة هنا، سيتم إجراء ذلك تلقائيا.
- يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل OneNote الملفات) يدويا.
- Project قد تحتاج مواقع الخوادم إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح. 
