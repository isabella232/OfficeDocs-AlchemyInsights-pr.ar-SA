---
title: 0x8004de40 خطأ عند تشغيل OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: e329d7fe881a0fc9514584e06aa2d6e8ebab5b11
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813639"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 خطأ عند تشغيل OneDrive

إذا تلقيت رسالة خطأ **0x8004de40** عند تسجيل الدخول إلى OneDrive، ف إعادة تشغيل الكمبيوتر أثناء الاتصال بمجال العمل أو المدرسة. إذا تلقيت هذا الخطأ بعد إعادة التشغيل، فجرب ذلك أثناء الاتصال بمجال العمل أو المدرسة:

1. انقر فوق بدء، وا اكتب **cmd** أو **موجه الأوامر**  في مربع البحث، وانقر بيمين فوق تطبيق موجه الأوامر، وحدد  **تشغيل كمسؤول**. إذا تم مطالبتك بكلمة مرور المسؤول أو للتأكيد، فا اكتب كلمة المرور، أو انقر فوق **السماح**.  

2. في نافذة موجه الأوامر، اكتب **dsregcmd/leave**  وانتظر حتى اكتمال الأمر. ثم اكتب **dsregcmd /join** وانتظر حتى اكتمال الأمر.
3. إعادة تشغيل الكمبيوتر.
