---
title: البحث عن التطبيقات المفقودة على شفرة تسجيل التطبيق
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404141"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>البحث عن التطبيقات المفقودة على شفرة تسجيل التطبيق

1. يتعذر العثور على التطبيقات على مدخل تسجيل التطبيق.

    إذا كان أحد التطبيقات تطبيقا متعدد المستأجرين وكان مسجلا في مستأجر آخر، لن يتم عرضه ضمن شفرة تسجيل التطبيق. ومع ذلك، قد تجده ضمن شفرة تطبيقات المؤسسة بمجرد الوصول إليها (بعد الموافقة عليها) وقد تم إنشاء الخدمة الأساسية في المستأجر الخاص بك. لمزيد من المعلومات، راجع [تطبيقات & الأساسية للخدمة في Azure AD - النظام الأساسي لهوية Microsoft](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. يتعذر عرض التطبيقات في شفرة تسجيل التطبيق على الرغم من أنك مسؤول.

    الرجاء التأكد من وجودك في الدليل الصحيح على مدخل Azure.
3. تطبيقي غير مدرج ضمن شفرة تطبيقات المؤسسة ولكنه يظهر عند استعلام أمر PowerShell.

    في بعض الأحيان، بعد حذف التطبيق من مدخل Azure، لا يظهر التطبيق في المدخل ولكن ربما لم يتم حذفه بالكامل. لمزيد من المعلومات، اطلع على:
    - يمكنك استرداد قائمة التطبيقات المحذوفة مسبقا وترى ما إذا كان التطبيق يظهر في القائمة باستخدام الأمر Powershell: **Get-AzureADDeletedApplication**. لمعرفة المزيد، راجع [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - إذا كنت تريد إزالة التطبيق بالكامل، يمكنك تجربة ما يلي في PowerShell: **Remove-AzureADApplication -ObjectId**. لمعرفة المزيد، راجع [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - بدلا من ذلك، يمكنك محاولة استعادة التطبيق المحذوف باستخدام الأمر Powershell التالي: **استعادة AzureADDeletedApplication -ObjectId**. لمعرفة المزيد، راجع [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. لا يمكنني العثور على قائمة بكل تطبيقات المؤسسة المثبتة مسبقا في مستأجر Azure الجديد.

    لا توجد تطبيقات مؤسسة مثبتة مسبقا في Azure AD بشكل افتراضي. ستحتاج إلى إضافته يدويا من الخيار "تطبيق جديد" من خلال استعراضه من معرض Azure AD أو إضافة تطبيق غير معرض. لمعرفة المزيد، راجع "الاستخدام السريع": إضافة تطبيق إلى مستأجر [Azure Active Directory (Azure AD).](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    إذا كنت مسؤولا عاما، يمكنك الوصول بسهولة إلى تطبيقاتك باستخدام [Microsoft 365 App Launcher](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. تعذر العثور على تطبيقاتي من مدخل "التطبيقات".

    تأكد من عدم إخفاء التطبيقات في صفحة مجموعة تطبيقاتي. لمعرفة المزيد، راجع [المجموعات (معاينة) في مدخل التطبيقات - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. لبدء التطبيقات من مدخل تطبيقاتي، راجع تحديد & استخدام التطبيقات على مدخل التطبيقات [- Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. لا يظهر تطبيق Office 365 Mover على شفرة تطبيقات المؤسسة بعد التثبيت.

    تطبيق "Office 365 Mover" هو تطبيق متعدد الاستخدامات لا يحتاج إلى إضافة إلى AAD باستخدام المقطع تطبيقات المعرض ضمن تسجيل تطبيقات المؤسسة. للوصول إلى تطبيق Office 365 Mover، ما عليك سوى تسجيل الدخول إلى التطبيق وطلب موافقة المستخدم على الأذونات. بمجرد أن يقدم المستخدم الموافقة، سيضاف هذا التطبيق تلقائيا إلى المستأجر باستخدام عنوان البريد الإلكتروني الذي سجلت دخوله.

    بعد تسجيل الدخول إلى التطبيق، يجب أن تتمكن من العثور على إدخال هذا التطبيق ضمن النصل تطبيقات المؤسسة في AAD. تحتاج إلى البحث عن هذا التطبيق إما بكتابة الاسم الكامل، أي "Office 365 Mover" أو البحث ببساطة عن "office" ويجب أن يتم سرد التطبيق. لمعرفة المزيد، [راجع Office 365 Mover](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)يقول إنه مثبت بالفعل ولكنه غير مدرج في معرض تطبيقات المؤسسة .
8. تشغيل سريع: عرض قائمة التطبيقات التي تستخدم مستأجر [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) لإدارة الهويات يوضح لك كيفية عرض التطبيقات، المعروفة أيضا باسم التطبيقات، التي تم إعدادها بالفعل لاستخدام مستأجر Azure AD كموفر الهوية (IdP).
9. يساعدك استكشاف الأخطاء الشائعة وإصلاحها عند إضافة تطبيق إلى [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) أو إزالته على فهم المشاكل الشائعة التي يواجهها الأشخاص عند عرض التطبيقات في Azure Active Directory.
