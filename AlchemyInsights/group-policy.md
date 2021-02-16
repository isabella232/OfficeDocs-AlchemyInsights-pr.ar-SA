---
title: نهج المجموعة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8303"
- "9003234"
ms.openlocfilehash: a829a78bbe947300b6dabb9fdb36088c17809742
ms.sourcegitcommit: 6900c2b7208ca51a9873dfc2e00be6f66cb25e3c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/15/2021
ms.locfileid: "50256651"
---
# <a name="group-policy"></a>نهج المجموعة

غالبا ما تدار إعدادات كائنات المستخدم والكمبيوتر في Azure Active Directory Domain Services (Azure AD DS) باستخدام كائنات نهج المجموعة (GPOs). يتضمن Azure AD DS "GPOs" مضمنا لمستخدمي AADDC والحاويات "أجهزة كمبيوتر AADDC". يمكنك تخصيص هذه الإعدادات المضمنة ل GPOs لتكوين نهج المجموعة كما هو مطلوب بيئة. لدى أعضاء مجموعة مسؤولي Azure AD DC امتيازات إدارة نهج المجموعة في مجال Azure AD DS، ويمكنهم أيضا إنشاء وحدات GPOs ووحدات تنظيمية مخصصة. لمزيد من المعلومات حول نهج المجموعة وكيفية عمله، راجع نظرة عامة [حول "نهج المجموعة".](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

في بيئة مختلطة، لا يتم مزامنة سياسات المجموعات التي تم تكوينها في بيئة AD DS المحلية مع Azure AD DS. لتعريف إعدادات التكوين للمستخدمين أو أجهزة الكمبيوتر في Azure AD DS، قم بتحرير أحد "برامج GPOs" الافتراضية أو قم بإنشاء "نقطة GPO" مخصصة.

توضح [لك](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) هذه المقالة "إدارة نهج المجموعة" كيفية تثبيت أدوات "إدارة نهج المجموعة"، وكيفية تحرير "أدوات إدارة نهج المجموعة" المضمنة، وكيفية إنشاء "أدوات إدارة نهج المجموعة" المخصصة.



