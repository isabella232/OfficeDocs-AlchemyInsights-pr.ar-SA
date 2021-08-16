---
title: نشر GPO
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: 6f9e164713ce36023de954d45031fd4414780e174bf5c7741c4aec274a65b32e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54067827"
---
# <a name="gpo-deployment"></a>نشر GPO

الإعدادات إدارة العناصر الخاصة ب المستخدم والكمبيوتر في Azure Active Directory Domain Services (Azure AD DS) غالبا باستخدام كائنات نهج المجموعة (GPOs). يتضمن Azure AD DS GPOs مضمنا في حاويات مستخدمي AADDC وأجهزة كمبيوتر AADDC. يمكنك تخصيص هذه الإعدادات المضمنة ل GPOs لتكوين نهج المجموعة كما هو مطلوب لبيئة. لدى أعضاء مجموعة مسؤولي Azure AD DC امتيازات إدارة نهج المجموعة في مجال Azure AD DS، ويمكنهم أيضا إنشاء وحدات GPOs مخصصة ووحدات تنظيمية (OUs). لمزيد من المعلومات حول نهج المجموعة وكيفية عمله، راجع [نظرة عامة حول نهج المجموعة](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11)).

في بيئة مختلطة، لا يتم مزامنة سياسات المجموعة التي تم تكوينها في بيئة AD DS المحلية إلى Azure AD DS. لتعريف إعدادات التكوين للمستخدمين أو أجهزة الكمبيوتر في Azure AD DS، قم بتحرير أحد مواقع GPOs الافتراضية أو قم بإنشاء GPO مخصص.

توضح [لك](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) هذه المقالة إدارة نهج المجموعة كيفية تثبيت أدوات "إدارة نهج المجموعة"، وكيفية تحرير "أدوات إدارة نهج المجموعة" المضمنة، وكيفية إنشاء "GPOs" مخصصة.
