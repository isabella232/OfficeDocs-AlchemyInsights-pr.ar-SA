---
title: أنتيسبام-5.7.23
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3156"
- "9001196"
ms.openlocfilehash: ecbce4f0077dc9acab63575c19d40c0675a406ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47717312"
---
# <a name="fix-email-delivery-issues-for-error-code-5723"></a>إصلاح مشاكل تسليم البريد الكتروني لرمز الخطا 5.7.23

تاكد من ان سجل DNS SPF لمجالك لديك بشكل عام SPF أو مدقق سجلات DNS علي الويب.

تاكد من ان الرسالة الصادرة لم يتم تحديدها كبريد عشوائي بواسطة Microsoft وموجهه عبر [تجمع التسليم عالي الجودة](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages). لن تنجح الرسائل الموجودة في تجمع التسليم عالي المخاطرة في إيداع SPF ، التالي لن يتم قبولها بواسطة مؤسسه البريد الكتروني الوجهة.

إذا استمرت المشكلة ، فقد تحتاج إلى الاتصال بمسؤول مضيف البريد الذي تحاول إرسال البريد الكتروني اليه. قم بتدوين الخطا الخارجي المفصل المتوفر في رسالة وثبات. قد لا يتمكن دعم Microsoft من المساعدة.
