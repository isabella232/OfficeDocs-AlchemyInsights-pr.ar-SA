---
title: مشكله في فتح الملفات أو تنزيلها في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695636"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>مشكله في فتح الملفات أو تنزيلها في Yammer

يدعم Yammer الكلاسيكي خيارات متعددة لتحميل الملفات إلى الرسائل والمجموعات. وفقا لتكوين الشبكة ، الملفات الافتراضية للتخزين في SharePoint.

لا يدعم منتقي الملفات في Yammer الجديد بعد كل الخيارات المتوفرة في Yammer الكلاسيكي. سيقوم التحديث المستقبلي باضافه ميزات اضافيه. للحصول علي مزيد من المعلومات ، راجع [إرفاق ملف أو صوره بمنشور محادثه Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**تعذر فتح ملف أو تنزيله**  

قد يتم تحميل ملف إلى Yammer ولكنه أيضا يكون مرتبطا بملف في SharePoint Online. لاستكشاف الأخطاء وإصلاحها ، يجب عليك أولا تحديد موقع الملف. إذا تم تحميل الملف إلى Yammer ، سيكون لديه عنوان URL * yammer.com. تاكد من إلغاء حظر عناوين Url و IP المطلوبة. للحصول علي مزيد من المعلومات ، راجع منشور المدونة [باستخدام عناوين IP المرمزة بشكل ثابت ل Yammer غير مستحسن](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

تحقق مما إذا كان بإمكان المستخدم الذي يملك المسؤول العام تنزيل الملف. إذا كان الملف خاصا ، فقد تحتاج إلى استخدام وضع المحتوي الخاص. للحصول علي مزيد من المعلومات ، راجع [عرض المحتوي الخاص في Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer علي مستوي الشبكة والملفات في SharePoint Online**  

لا تستخدم [الضيوف علي مستوي الشبكة في Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) الخاص ب AZURE AD B2B وتكون داخلية لخدمه yammer ، التالي لا يمكنهم الوصول إلى ملفات yammer المخزنة في SharePoint. يمكنك إنشاء مستخدم خاص بموقع AAD الخارجي الذي يمكنه الوصول إلى مكتبات المستندات في SharePoint Online باستخدام تلك الهوية. للحصول علي معلومات حول دعم الضيوف المستقبلي في Azure AD B2B في Yammer ، راجع [دعم الضيف للشركات (B2B) في معاينه Yammer-شروط العميل والاسئله المتداولة](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).