---
title: تمكين Office 365 ATP SharePoint وأندريف وفرق Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/02/2019
ms.locfileid: "31030870"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>تمكين الحماية من التهديدات المتقدمة 365 Office SharePoint على الإنترنت وأندريف وفرق Microsoft

1. اذهب إلى https://protection.office.com وتسجيل الدخول.
2. اختر **إدارة التهديد** > **نهج** > **مرفقات آمنة**.
3. حدد **تشغيل ATP لفرق Microsoft SharePoint وأندريف،** ومن ثم انقر فوق **حفظ**.
4. (مستحسن) مسؤول عمومي أو كمسؤول SharePoint على الإنترنت، تشغيل cmdlet [سبوتينانت مجموعة](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) باستخدام المعلمة **ديسالووينفيكتيدفيليدوونلواد** تعيين إلى *true*.
5. (مستحسن) [إعداد تنبيهات](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) للملفات التي تم الكشف عنها.

> [!NOTE]
> سيتم ATP n ولفحص كل ملف واحد في SharePoint على الإنترنت أو أندريف أو فرق Microsoft. يتم تفحص الملفات بشكل غير متزامن، من خلال عملية تستخدم الأحداث نشاط المشاركة وضيوف، جنبا إلى جنب مع إشارات التهديد للتعرف على الملفات الضارة والأساليب البحثية الذكية. راجع [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).