---
title: التكوين الظاهري مع خدمات مجال AAD
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884803"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>التكوين الظاهري مع خدمات مجال AAD

يشمل التكوين الافتراضي مع خدمات مجال AAD الخطوات التالية: 

1. التحقق من صحة المجال علي مدخل Azure https://aka.ms/aadds-health
2. التحقق من نسجك عن القواعد التي تحظر المنافذ المطلوبة لاجراء المزامنة في خدمات مجال Azure AD علي المدخل https://aka.ms/aadds-networking
3. التاكد من ان الشبكة الظاهرية لديك يتم نشرها في نفس منطقه Azure الخاصة بالمجالات المدارة في Azure AD.
4. التاكد من انك لا تملك مجالا موجودا باسم المجال نفسه المتوفر علي الشبكة الافتراضية.

للحصول علي مزيد من التفاصيل حول اعتبار التصميم علي الشبكة الظاهرية في Azure لدعم خدمات مجالات AAD ، راجع [اعتبارات الشبكة الظاهرية](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).

