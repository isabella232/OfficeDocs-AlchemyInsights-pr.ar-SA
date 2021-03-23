---
title: الاستيراد والتصدير من Yammer
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/19/2021
ms.locfileid: "51034792"
---
# <a name="import-and-export-from-yammer"></a>الاستيراد والتصدير من Yammer

**استيراد**

تختلف خيارات استيراد المستخدم استنادا إلى ما إذا كانت Yammer الشبكة في الوضع الأصلي [ل Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)أو لا.

- **الوضع غير** الأصلي : يمكن استيراد المستخدمين إلى مجموعات باستخدام إضافة من دفتر العنوان [(حد](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) 100 [](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) مستخدم) ضمن إعدادات المجموعة، أو إلى الشبكة باستخدام التحديث المجمع داخل مسؤول الشبكة.
- **الوضع الأصلي**: يجب تنفيذ عمليات عضوية المجموعة وعضوية الشبكة من مدخل [مسؤول Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users)، مدخل [Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)، أو باستخدام خيار Azure AD آخر. لم تعد الشبكات في الوضع الأصلي قادرة على الوصول إلى التحديث المجمع والميزات القديمة الأخرى.

> [!IMPORTANT]
> Yammer أي دعم لاستيراد محتوى من داخل مسؤول الشبكة حتى عند استخدام ميزة "تصدير البيانات" في شبكة أخرى. يمكن إعادة نشر المحتوى بواسطة حلول الشركاء أو Yammer واجهات برمجة التطبيقات REST.

**تصدير**

[يسمح تصدير بيانات الشبكة ضمن مسؤول](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) الشبكة بتصدير المحتوى من Yammer، بما في ذلك الرسائل والملفات. يمكن أن تكون المرفقات كبيرة جدا وستتسبب في أن تستغرق عمليات التصدير وقتا طويلا لإكمالها. نوصي بتصدير الشبكات النشطة باستخدام [API لتصدير](https://developer.yammer.com/docs/data-export-api) البيانات في أجزاء حسب اليوم أو الأسبوع. لا يوفر دعم Microsoft برامج نصية مخصصة لهذا الغرض.

يوجد تصدير [القانون العام لحماية البيانات (GDPR)](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) منفصل لتصدير المحتوى لمستخدم فردي.