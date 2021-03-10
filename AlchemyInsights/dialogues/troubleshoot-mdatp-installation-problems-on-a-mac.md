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
ms.openlocfilehash: 4b03361666f950a2010e4c4d8e78d156438d9e90
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/09/2021
ms.locfileid: "50692628"
---
# <a name="troubleshoot-mdatp-installation-problems-on-a-mac"></a>استكشاف مشاكل تثبيت MDATP وإصلاحها على جهاز Mac

إذا فشل التثبيت اليدوي، **تظهر** صفحة الملخص لمعالج التثبيت الخطأ التالي:

"حدث خطأ أثناء التثبيت. واجه المثبت خطأ تسبب في فشل التثبيت. اتصل بالشركة المصنعة للبرنامج للحصول على المساعدة."

بالنسبة إلى عمليات نشر MDM، تظهر الصفحة أيضا فشلا عاما في التثبيت.

على الرغم من أننا لا نعرض أخطاء دقيقة للمستخدمين النهائيين، إلا أننا نحتفظ بملف سجل مع تقدم عملية التثبيت، في **/Library/Logs/Microsoft/mdatp/install.log.** يتم إلحاق كل جلسة عمل تثبيت إلى ملف السجل هذا. إخراج جلسة التثبيت الأخيرة فقط، استخدم `sed` .

لمعرفة المزيد، راجع استكشاف مشاكل التثبيت وإصلاحها [ل Microsoft Defender ATP for Mac.](https://go.microsoft.com/fwlink/?linkid=2144615)
