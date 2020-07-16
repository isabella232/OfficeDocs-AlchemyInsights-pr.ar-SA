---
title: مشكلة فتح الملفات أو تنزيلها في Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: 6dfcbe9abfc23219a61e81785d31c11f7a0fa95c
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148168"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>مشكلة فتح الملفات أو تنزيلها في Yammer

يدعم Yammer الكلاسيكي خيارًا متعددًا لتحميل الملفات إلى الرسائل والمجموعات. اعتماداً على تكوين شبكة الاتصال، الافتراضي الملفات إلى التخزين في SharePoint.

لا يعتمد منتقي الملفات في Yammer الجديدة بعد كافة الخيارات المتوفرة في Yammer الكلاسيكية. سوف يضيف التحديث المستقبلي ميزات إضافية. لمزيد من المعلومات، راجع [إرفاق ملف أو صورة إلى مشاركة محادثة Yammer](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**تعذر فتح ملف أو تنزيله**  

قد يتم تحميل ملف إلى Yammer ولكن أيضاً الارتباط بملف في SharePoint Online. لاستكشاف الأخطاء وإصلاحها، يجب أولاً تحديد موقع الملف. إذا تم تحميل الملف إلى Yammer، سيكون له عنوان URL *.yammer.com. تأكد من إلغاء حظر عناوين URL وعناوين IP المطلوبة. لمزيد من المعلومات، راجع نشر المدونة [باستخدام عناوين IP المشفرة الثابتة لـ Yammer غير مستحسن](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

تحقق من ما إذا كان بإمكان المستخدم الذي هو مسؤول عمومي أيضًا تنزيل الملف. إذا كان الملف خاصًا، قد تحتاج إلى استخدام وضع المحتوى الخاص. لمزيد من المعلومات، راجع ثم [مراقبة المحتوى الخاص في Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Yammer على مستوى الشبكة الضيوف والملفات في SharePoint عبر الإنترنت**  

لا يستخدم [الضيوف على مستوى الشبكة في Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) Azure AD B2B وهم داخليون لخدمة Yammer، بحيث لا يمكنهم الوصول إلى ملفات Yammer المخزنة في SharePoint. إنشاء مستخدم AAD B2B خارجي الذين يمكنهم الوصول إلى مكتبات المستندات في SharePoint عبر الإنترنت باستخدام تلك الهوية. للحصول على معلومات حول دعم ضيف Azure A2B في Yammer، راجع [دعم الضيف بين الشركات (B2B) في Yammer Preview - شروط العملاء والأسئلة الشائعة](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).