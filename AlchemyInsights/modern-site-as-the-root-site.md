---
title: الموقع الحديث كموقع الجذر
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 04/21/2020
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 0388f95e2b7815dcbbb6aca200f44e55e9c5724f
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43713778"
---
# <a name="modern-site-as-root-site"></a>الموقع الحديث كموقع الجذر

لقد بدأنا في طرح ميزة جديدة من شأنها أن تسمح لك [لمبادلة موقع جذر الموقع الكلاسيكي الخاص بك مع موقع حديث.](https://docs.microsoft.com/sharepoint/modern-root-site) استخدم [Invoke-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع موقع مع موقع آخر أثناء أرشفة الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعة) وموقع الاتصال.

>[!Important]
> لا تقم بحذف موقع الجذر الكلاسيكي الخاص بك لإنشاء موقع اتصال حديث. هذا غير معتمد من قبل Microsoft. سيؤدي حذف موقع الجذر إلى جعل جميع مواقع SharePoint في مؤسستك غير قابلة للوصول إلى جميع المستخدمين، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في نفس عنوان URL. سنقوم بتوصيل هذه الميزة عبر مركز الرسائل. يجب أن تتوقع تشغيل الميزة في المستأجر الخاص بك قريباً.

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع مواقع المبادلة
- قد يرجع الموقع المستهدف خطأ "لم يتم العثور عليه" (HTTP 404) لفترة قصيرة من الزمن.
- يجب إعادة كتابة المحتوى لتحديث فهرس البحث. لا توجد خطوة يدوية مطلوبة هنا ، وسيتم ذلك تلقائيا.
- أي شيء يعتمد على الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سيحتاج إلى تصحيح يدويًا.
- قد تحتاج مواقع Project Server إلى التحقق من صحتها للتأكد من أنها لا تزال مقترنة بشكل صحيح. 
