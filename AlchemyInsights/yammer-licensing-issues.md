---
title: مشاكل الترخيص في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657263"
---
# <a name="yammer-licensing-issues"></a>مشاكل الترخيص في Yammer

يجب ان يتوفر لدي جميع المستخدمين ترخيص لاستخدام خدمه Yammer Enterprise ، ولكن لا يتطلب Yammer الافتراضي ان يملك المستخدمون ترخيصا للوصول إلى الخدمة. عندما يقوم مسؤول بتغيير الاعداد لحظر مستخدمي Microsoft 365 بدون تراخيص Yammer ، لن يتمكن المستخدمون من تعيين ترخيص Yammer Enterprise علي خدمه Yammer. لمزيد من المعلومات ، راجع [أداره تراخيص مستخدم Yammer في Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) 

عند أزاله التراخيص من المستخدمين ، لم تعد لوحه Yammer معروضه ، ويمكن للخدمات الأخرى استخدام أزاله الترخيص لإخفاء الميزات. في بعض الحالات الأخرى ، لا يزال بإمكان الميزات ان تظهر ولكنه يتطلب تعيين ترخيص للعمل.  

**لم يتم تحديث الترخيص للمستخدم**  

في بعض الأحيان ، يتم تعيين ترخيص للمستخدم ولكن لا يزال يتعذر عليك الوصول إلى Yammer. من المحتمل ان تحدث التاخيرات في حاله تقدم تعيين ترخيص كبير. قد لا يتم تحديث مستخدمي Yammer بنفس الترتيب حيث يتم تغيير التراخيص في Azure AD لان النظام يعمل بشكل غير متزامن. يمكنك الانتظار لمده 24 ساعة قبل فتح حاله دعم للإبلاغ عن مشاكل مزامنة الترخيص.  

**تعيين ترخيص مجمع**  

يمكن تعيين التراخيص من خلال مركز الاداره أو البرمجة النصية ل PowerShell. لمزيد من المعلومات ، راجع [تعيين تراخيص للمستخدمين](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [وتعيين تراخيص لحسابات المستخدمين باستخدام Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell). 

لا يوفر دعم Microsoft المساعدة في إنشاء البرامج النصية ، ولكن تتوفر الوثائق الموجودة علي تعيين ترخيص Yammer. لمزيد من المعلومات ، راجع [أداره تراخيص Yammer باستخدام Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).