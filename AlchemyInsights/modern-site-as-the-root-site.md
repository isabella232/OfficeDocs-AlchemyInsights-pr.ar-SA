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
ms.openlocfilehash: a0f48dc79b51168c9cc045078ad8fc7d668343c7
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327589"
---
# <a name="modern-site-as-root-site"></a>الموقع الحديث كم موقع الجذر

لقد بدأنا في طرح ميزة جديدة تسمح لك بتبادلة موقع الجذر الكلاسيكي الخاص بك [مع موقع حديث](https://docs.microsoft.com/sharepoint/modern-root-site). استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع بموقع آخر أثناء أرشفة الموقع الأصلي. يتوفر لكل من موقع الفريق (غير متصل بمجموعة) و"موقع الاتصالات".

**هام**: لا تحذف موقعك الجذر الكلاسيكي لإنشاء موقع اتصالات حديث. لا تدعم Microsoft هذا الأمر. من خلال حذف الموقع الجذر، لن SharePoint الوصول إلى كل المواقع في مؤسستك من قبل جميع المستخدمين، حتى تستعيد الموقع أو تنشئ موقعا جديدا في عنوان URL نفسه. سنقوم بتواصل هذه الميزة عبر مركز الرسائل. يجب أن تتوقع تشغيل الميزة في المستأجر الخاص بك قريبا.

## <a name="known-issues-with-swapping-sites"></a>المشاكل المعروفة في تبديل المواقع
- قد يرجع الموقع الهدف الخطأ "لم يتم العثور عليه" (HTTP 404) لفترة زمنية قصيرة.
- يجب إعادة فهرسة المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة هنا، سيتم إجراء ذلك تلقائيا.
- يجب تصحيح أي شيء يعتمد على الارتباطات "الثابتة" (مثل OneNote الملفات ومزامنة الملفات) يدويا.
- Project قد تحتاج مواقع الخوادم إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح. 
