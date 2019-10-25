---
title: مضاد البريد المزعج-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: 9c9bc2d04fb8efaa5e75194b4ca09316d24e018e
ms.sourcegitcommit: 07b47d7f3ca191363e6bc84140e8e01524d6f08e
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 10/24/2019
ms.locfileid: "37682016"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشكلات تسليم البريد الكتروني لرمز الخطا 5.7.23

تحقق من سجل DNS SPF للمجال الخاص بك في مدقق سجلات SPF أو DNS المتوفرة للعامة علي الويب.

تحقق من ان الرسالة الصادرة لم يتم تعريفها كرسائل غير مرغوب فيها بواسطة Office 365 وتوجيهها عبر [تجمع التسليم عالي المخاطر](https://docs.microsoft.com/office365/SecurityCompliance/high-risk-delivery-pool-for-outbound-messages). الرسائل في تجمع التسليم عاليه المخاطر لن تمر الشيكات SPF ، التالي لن تكون مقبوله من قبل مؤسسه البريد الكتروني الوجهة.

إذا استمرت المشكلة ، قد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الكتروني. قم بتدوين الخطا الخارجي المفصل المتوفر في رسالة الارتداد.  قد لا يتمكن دعم Office 365 من المساعدة بشكل أكبر.