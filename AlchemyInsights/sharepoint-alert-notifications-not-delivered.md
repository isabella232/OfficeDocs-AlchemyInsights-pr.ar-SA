---
title: لم يتم تسليم اعلامات تنبيه SharePoint
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 978ca8df40736228932ae6f6a7c33ad0b159d4e5
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2019
ms.locfileid: "40047054"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>لم يتم تسليم اعلامات تنبيه SharePoint

يرجى التحقق من المجلد غير المرغوب فيه في البريد الكتروني الخاص بك ، كما في بعض الأحيان قد تذهب التنبيات هناك.

تحديد ما إذا **لم يتم تسليم كافة التنبيات** أو إذا لم يتم تسليم **تنبيه فردي** من ملف أو مكتبه معينه.

- **لا يتم تسليم التنبيات الفردية**: إذا لم يتم تسليم تنبيه فردي من ملف أو مكتبه معينه ، يمكنك محاولة حذفه وأعاده إنشائه. راجع [أداره تنبيات SharePoint أو عرضها أو حذفها](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2?ui=en-US&rs=&ad=US#ID0EAADAAA=Online) لأعاده إنشاء التنبيه.
- **لا يتم تسليم كافة التنبيات**: إذا لم يتم تسليم كافة التنبيات من ملفات أو مكتبات متعددة ، قم بزيارة [لوحه معلومات "صحة الخدمة](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) " للتحقق من وجود إيه تنبيات/الاحداث التي قد تحدث مع SharePoint أو Exchange. قد تكون المشكلة مع امكانيه التنبيه SharePoint أو التاخير في رسائل البريد الكتروني من خلال Exchange. سيكون من المهم أيضا ان نلاحظ ما إذا كان يتم تسليم البريد الكتروني الأخرى ، وإذا لم يكن كذلك ، فان المشكلة من المحتمل مع تاخيرات Exchange.

التعليمات حول التنبيات:

- من غير الممكن إرسال تنبيات إلى "مجموعه التوزيع" ، يتم اعتماد مجموعات الأمان و O365 فقط.
- لا يمكنك تخصيص قوالب البريد الكتروني التنبيه; تحتاج إلى استخدام Microsoft FLOW أو SharePoint مصمم سير العمل لتحقيق تلك.

مزيد من المعلومات:

- **اعداد التنبيه**: لمزيد من المعلومات حول اعداد التنبيات ، راجع [إنشاء تنبيه للحصول علي اعلام عند تغيير ملف أو مجلد في SharePoint](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918).
- **استكشاف أخطاء التنبيات وإصلاحها**: لمزيد من المعلومات حول استكشاف أخطاء التنبيات وإصلاحها ، راجع [المستخدمين لا يتلقون اعلامات تنبيه SharePoint علي الإنترنت](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications).
- **نهج تنبيه الامتثال لO365 المتقدمة**: لمزيد من المعلومات حول اعداد هذه التنبيات ، راجع [نهج تنبيه التوافق](https://docs.microsoft.com/office365/securitycompliance/alert-policies).
- **سجلات التدقيق في SharePoint و OneDrive**: لمزيد من المعلومات حول كيفيه استرداد هذه الاحداث ، راجع [البحث في سجل التدقيق](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
- **التنبيات المرسلة بواسطة الحماية المتقدمة للتهديد**: راجع [ATP ل SharePoint و OneDrive](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).
- **التنبيات المرسلة بواسطة سياسات منع فقدان البيانات**: راجع [اعلامات البريد الكتروني لنهج DLP](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).

## <a name="related-topics"></a>مواضيع ذات صله

هل تريد محاولة Microsoft Flow في SharePoint علي الإنترنت ؟

- [إنشاء تدفق](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint والتدفق](https://flow.microsoft.com//blog/sharepoint-and-flow/)
