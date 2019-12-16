---
title: الموقع الحديث كموقع الجذر
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.date: 8/7/2019
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000265"
- "1874"
ms.openlocfilehash: 2e2bb02b9dbaf7f8ede0b4c5ba8c8f29453309cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054689"
---
# <a name="modern-site-as-root-site"></a>الموقع الحديث كموقع الجذر

لقد بدانا في طرح ميزه جديده من شانها ان تسمح لك [لمبادله موقع الجذر موقع الكلاسيكية الخاصة بك مع موقع حديث](https://docs.microsoft.com/sharepoint/modern-root-site). استخدام [استدعاء-SPOSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) لمبادله موقع موقع مع موقع آخر اثناء أرشفه الموقع الأصلي. متوفر لكل من موقع الفريق (غير متصل بمجموعه) وموقع الاتصالات.

>[!Important]
> لا تحذف موقع الجذر الكلاسيكي الخاص بك لإنشاء موقع اتصالات حديث. هذا غير معتمد من قبل Microsoft. سيؤدي حذف موقع الجذر إلى جعل كافة مواقع SharePoint في مؤسستك غير قابله للوصول إلى كافة المستخدمين ، حتى تقوم باستعادة الموقع أو إنشاء موقع جديد في نفس عنوان URL. سنقوم بتوصيل هذه الميزة عبر مركز الرسائل. يجب ان تتوقع ان يتم تشغيل الميزة في المستاجر الخاص بك قريبا.

## <a name="known-issues-with-swapping-sites"></a>المشكلات المعروفة مع تبادل المواقع
- قد يرجع الموقع الهدف خطا "لم يتم العثور علي" (HTTP 404) لفتره قصيرة من الوقت.
- سيحتاج المحتوي إلى أعاده التصنيف لتحديث فهرس البحث. لا توجد خطوه يدوية مطلوبه هنا ، سيتم ذلك تلقائيا.
- اي شيء يعتمد علي الارتباطات "الثابتة" (مثل مزامنة الملفات وملفات OneNote) سوف تحتاج إلى تصحيح يدويا.
- قد تحتاج مواقع خادم Project إلى التحقق من صحتها للتاكد من انها لا تزال مقترنة بشكل صحيح. 
