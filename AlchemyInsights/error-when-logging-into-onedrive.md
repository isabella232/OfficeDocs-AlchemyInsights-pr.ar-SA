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
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946566"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>0x8004de40 خطأ عند تشغيل OneDrive

إذا تلقيت رسالة خطأ 0x8004de40 **تسجيل** الدخول إلى OneDrive، ف إعادة تشغيل الكمبيوتر أثناء الاتصال بمجال العمل أو المدرسة. إذا تلقيت هذا الخطأ بعد إعادة التشغيل، فجرب ذلك أثناء الاتصال بمجال العمل أو المدرسة:

1. انقر فوق بدء، وا اكتب **cmd** أو **موجه الأوامر**  في مربع البحث، وانقر بيمين فوق تطبيق موجه الأوامر، وحدد  **تشغيل كمسؤول**. إذا تم مطالبتك بكلمة مرور المسؤول أو للتأكيد، فا اكتب كلمة المرور، أو انقر فوق **السماح**.  

2. في نافذة موجه الأوامر، اكتب **dsregcmd/leave**  وانتظر حتى اكتمال الأمر. ثم اكتب **dsregcmd /join** وانتظر حتى اكتمال الأمر.
3. إعادة تشغيل الكمبيوتر.
