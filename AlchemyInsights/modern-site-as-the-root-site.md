---
title: حديث الموقع الجذر
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
ms.openlocfilehash: 2f75f1e60af06da47fe846e84bbb370dd60084e9
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/22/2019
ms.locfileid: "36543840"
---
# <a name="modern-site-as-root-site"></a>موقع الحديثة كالموقع الجذر

وقد بدأنا للتمهيد ميزة جديدة تسمح لك لتبديل موقع جذر الموقع التقليدي بموقع حديثة. استخدام [استدعاء سبسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موضع موقع بموقع آخر أثناء الأرشفة الموقع الأصلي. يتوفر لكل موقع الفريق (غير متصل بمجموعة) وموقع الاتصال. 

>[!Important]
> لا تقم بحذف الموقع الجذر الكلاسيكية لإنشاء "موقع الاتصالات" الحديثة. وهذا غير معتمد من قبل Microsoft. حذف الموقع الجذر سيجعل كافة مواقع SharePoint في المؤسسة الخاصة بك غير متاحة لكافة المستخدمين، حتى يمكنك استعادة الموقع أو إنشاء موقع جديد على نفس العنوان. أننا سوف يمكن الاتصال هذه الميزة عبر مركز الرسائل. يجب أن تتوقع ميزة تشغيل في جهاز المستأجر بعد قليل.

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة المتعلقة بتبادل المواقع
- موقع الهدف قد بإرجاع خطأ (HTTP 404) "لم يتم العثور على" لفترة قصيرة من الوقت.
- أن محتوى تتبع الارتباطات من جديد لتحديث فهرس البحث. خطوة اليدوية ليست مطلوبة هنا، هذا يتم إنجازه تلقائياً.
- أي شيء يعتمد على روابط "ثابتة" (مثل ملفات OneNote ومزامنة الملفات) ستحتاج إلى تصحيحه يدوياً.
- قد تحتاج مواقع المشروع على الخادم التحقق من صحة للتأكد من أنها لا يزال مرتبطاً بشكل صحيح. 
