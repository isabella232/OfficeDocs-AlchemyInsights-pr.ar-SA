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
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/03/2021
ms.locfileid: "50426947"
---
# <a name="gpo-deployment"></a>نشر GPO

غالبا ما تدار إعدادات كائنات المستخدم والكمبيوتر في Azure Active Directory Domain Services (Azure AD DS) باستخدام كائنات نهج المجموعة (GPOs). يتضمن Azure AD DS "GPOs" مضمنا لمستخدمي AADDC والحاويات "أجهزة كمبيوتر AADDC". يمكنك تخصيص هذه الإعدادات المضمنة في GPOs لتكوين نهج المجموعة كما هو مطلوب بيئة. لدى أعضاء مجموعة مسؤولي Azure AD DC امتيازات إدارة نهج المجموعة في مجال Azure AD DS، ويمكنهم أيضا إنشاء وحدات GPOs ووحدات تنظيمية مخصصة. لمزيد من المعلومات حول نهج المجموعة وكيفية عمله، راجع [نظرة عامة حول نهج المجموعة.](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))

في البيئة المختلطة، لا يتم مزامنة سياسات المجموعات التي تم تكوينها في بيئة AD DS المحلية مع Azure AD DS. لتعريف إعدادات التكوين للمستخدمين أو أجهزة الكمبيوتر في Azure AD DS، قم بتحرير أحد "برامج GPOs" الافتراضية أو قم بإنشاء "نقطة GPO" مخصصة.

توضح لك هذه المقالة ["إدارة](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy) نهج المجموعة" كيفية تثبيت أدوات "إدارة نهج المجموعة"، وكيفية تحرير "أدوات إدارة نهج المجموعة" المضمنة، وكيفية إنشاء "أدوات إدارة نهج المجموعة" المخصصة.
