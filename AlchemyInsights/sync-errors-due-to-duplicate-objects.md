---
title: 902 (أخطاء المزامنة بسبب عناصر مكررة)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 75b684c5c6b4a594af069d8ed668df95726e1b31
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708049"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>أخطاء المزامنة بسبب عناصر مكررة

قد تتلقى واحدة من رسائل الخطأ التالية عند انتهاء مزامنة الدليل في Microsoft 365:

- يتعذر تحديث هذا الكائن في Microsoft Online Services لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بكائن آخر في الدليل المحلي.

- يوجد بالفعل كائن متزامن مع عنوان الوكيل نفسه في دليل Microsoft Online Services.

- يتعذر تحديث هذا الكائن لأن السمات التالية المقترنة بهذا الكائن لها قيم قد تكون مقترنة بالفعل بعائن آخر في خدمات الدليل المحلي: UserPrincipalName.

لتحديد المشكلة وإصلاحها، قم بتنزيل أداة معالجة الأخطاء [IdFix DirSync وتشغيلها.](https://github.com/Microsoft/idfix)

لمزيد من المعلومات، [راجع KB2647098.](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)
