---
title: إصلاح 0x8004de40 في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649735"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>إصلاح 0x8004de40 في OneDrive

إذا كنت تقوم بتشغيل Windows 7 وتلقيت هذا الخطأ، فحدث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .

إذا كنت تقوم بتشغيل Windows 10، وتلقيت رسالة خطأ 0x8004de40 OneDrive:

- إعادة تشغيل الكمبيوتر المتأثر أثناء الاتصال بمجال Acitve Directory.
- إذا لم تصلح عملية إعادة التشغيل المشكلة، ففك الانضمام إلى جهازك من Azure AD ثم إعادة الانضمام له. 

**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات. لا تقوم بتنفيذ هذه الخطوات عندما لا تكون متصلا بالبنية الأساسية الخاصة بالشركة (على سبيل المثال، أثناء السفر). 

1. افتح موجه أوامر غير مرفوط عن طريق تحديد **بدء،** وانقر ب زر الماوس الأيمن فوق **موجه الأوامر،** ثم حدد **تشغيل كمسؤول**.

1. اكتب *dsregcmd /leave واضغط* على **Enter**.

1. عند الإكمال، اكتب *dsregcmd /join واضغط* على **Enter**.

1. عند الانتهاء، أغلق موجه الأوامر.

1. إعادة تشغيل الكمبيوتر وتسجيل الدخول إلى OneDrive.