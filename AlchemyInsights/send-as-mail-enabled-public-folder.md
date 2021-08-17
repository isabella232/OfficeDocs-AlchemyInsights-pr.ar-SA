---
title: إرسال كمجلد عام ممكن للبريد في EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052553"
---
# <a name="sendas-mail-enabled-public-folder"></a>مجلد عام تم تمكين إرساله بالبريد

يعين المثال التالي أذونات "إرسال باسم" للمجلد العام الذي يمكن للبريد NewPF1 للمستخدم Jason.

Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'

للحصول على معلومات مفصلة حول بناء الجملة والمعلمات، راجع تعيين [أذونات "إرسال باسم"](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)أو "إرسال نيابة عن" للمجلدات العامة التي تم تمكين البريد لها.

