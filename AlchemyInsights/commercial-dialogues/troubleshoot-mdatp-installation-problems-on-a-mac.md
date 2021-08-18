---
title: استكشاف مشاكل تثبيت MDATP وإصلاحها على جهاز Mac
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
- "9000760"
- "7391"
ms.openlocfilehash: 4139f47f40a89069521aaa1a3e4fdab56e9e27a2096ae0ad099be827f60d51fc
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54090946"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>استكشاف مشاكل تثبيت MDATP وإصلاحها على جهاز Mac

إذا فشل التثبيت اليدوي، تظهر صفحة **الملخص** لمعالج التثبيت الخطأ التالي:

"حدث خطأ أثناء التثبيت. واجه المثبت خطأ تسبب في فشل التثبيت. اتصل بالشركة المصنعة للبرامج للحصول على المساعدة."

بالنسبة إلى عمليات نشر MDM، تظهر الصفحة فشلا عاما في التثبيت أيضا.

على الرغم من أننا لا نعرض أخطاء دقيقة للمستخدمين النهائيين، إلا أننا نحتفظ بملف سجل مع تقدم التثبيت، في **/Library/Logs/Microsoft/mdatp/install.log**. يتم إلحاق كل جلسة عمل تثبيت إلى ملف السجل هذا. لاخراج جلسة التثبيت الأخيرة فقط، استخدم `sed` .

لمعرفة المزيد، راجع استكشاف مشاكل التثبيت وإصلاحها [ل Microsoft Defender ATP for Mac](https://go.microsoft.com/fwlink/?linkid=2144615).
