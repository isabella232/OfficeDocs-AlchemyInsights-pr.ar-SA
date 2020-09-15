---
title: الموقع الحديث كالموقع الجذر
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
ms.openlocfilehash: 86ff5f7fbaed62de9047006bf4ba4d2db2be3def
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666857"
---
# <a name="modern-site-as-root-site"></a>موقع حديث كموقع جذر

لقد بدانا في نشر ميزه جديده ستسمح لك [بتبديل الموقع الجذر للموقع التقليدي مع موقع حديث](https://docs.microsoft.com/sharepoint/modern-root-site). استخدم [Invoke-سبوسيتيسواب](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لتبديل موقع الموقع مع موقع آخر اثناء أرشفه الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصال.

>[!Important]
> لا تحذف الموقع الجذر الكلاسيكي لإنشاء موقع اتصالات حديثه. لا يتم دعم هذا الأمر بواسطة Microsoft. سيؤدي حذف الموقع الجذر إلى جعل جميع مواقع SharePoint في مؤسستك غير قابله للوصول إلى كل المستخدمين ، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في عنوان URL نفسه. سنقوم بالاتصال بهذه الميزة عبر مركز الرسائل. يجب ان تتوقع ان تكون الميزة قيد التشغيل في نطاق المستاجر الخاص بك قريبا.

## <a name="known-issues-with-swapping-sites"></a>المشاكل المعروفة في مواقع التبادل
- قد يرجع الموقع الهدف الخطا "لم يتم العثور عليه" (HTTP 404) لفتره قصيرة من الوقت.
- سيحتاج المحتوي إلى ريكراوليد لتحديث فهرس البحث. لا توجد خطوه يدوية مطلوبه هنا ، سيتم تنفيذ ذلك تلقائيا.
- يجب تصحيح اي شيء يعتمد علي ارتباطات "static" (مثل مزامنة الملفات وملفات OneNote) يدويا.
- قد يلزم التحقق من صحة مواقع Project Server لضمان انها لا تزال مقترنة بشكل صحيح. 
