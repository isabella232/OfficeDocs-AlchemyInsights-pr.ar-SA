---
title: مشكلة في فتح الملفات أو تنزيلها في Yammer
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
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028237"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>مشكلة في فتح الملفات أو تنزيلها في Yammer

تدعم Yammer الكلاسيكية خيارات متعددة لتحميل الملفات إلى الرسائل والمجموعات. استنادا إلى تكوين الشبكة، يتم تخزين الملفات بشكل افتراضي في SharePoint.

لا يدعم منتقي الملفات في Yammer الجديدة جميع الخيارات المتوفرة في Yammer. سيضيف التحديث المستقبلي ميزات إضافية. لمزيد من المعلومات، راجع إرفاق ملف أو صورة إلى منشور Yammer [المحادثة.](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)

**تعذر فتح ملف أو تنزيله**  

قد يتم تحميل ملف Yammer ولكن يتم أيضا ربطه إلى ملف في SharePoint Online. لا استكشاف الأخطاء وإصلاحها، يجب أولا تحديد موقع الملف. إذا تم تحميل الملف إلى Yammer، سيكون له عنوان URL *.yammer.com URL. تأكد من إلغاء حظر عناوين URL وعناوين IP المطلوبة. لمزيد من المعلومات، راجع منشور المدونة استخدام عناوين IP البرمجية الأساسية [Yammer من المستحسن](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

تحقق مما إذا كان يمكن للمستخدم الذي هو أيضا مسؤول عام تنزيل الملف. إذا كان الملف خاصا، فقد تحتاج إلى استخدام وضع المحتوى الخاص. لمزيد من المعلومات، راجع بعد ذلك [مراقبة المحتوى الخاص في Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer ملفات وضيوف على مستوى الشبكة في SharePoint Online**  

[لا يستخدم](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) الضيوف على مستوى الشبكة في Yammer Azure AD B2B وهم داخليون في خدمة Yammer، لذا لا يمكنهم الوصول إلى ملفات Yammer المخزنة في SharePoint. قم بإنشاء مستخدم AAD B2B خارجي يمكنه الوصول إلى مكتبات المستندات في SharePoint عبر الإنترنت باستخدام تلك الهوية. للحصول على معلومات حول دعم ضيف Azure AD B2B المستقبلي في Yammer، راجع دعم الضيف من [Business-to-business (B2B) في Yammer Preview - شروط](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)العميل وال الأسئلة الشائعة.