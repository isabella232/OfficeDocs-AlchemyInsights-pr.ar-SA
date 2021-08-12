---
title: مشاكل مالك تسجيل التطبيق
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951120"
---
# <a name="app-registration-owner-issues"></a>مشاكل مالك تسجيل التطبيق

فيما يلي الأساليب المتوفرة لإضافة الأساسيات كملاك لتسجيلات التطبيقات:

- استخدام وحدة Azure AD PowerShell النمطية -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    المرجع: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- استخدام Azure CLI - `az ad app owner add`

    المرجع: [مالك تطبيق az ad](https://docs.microsoft.com/cli/azure/ad/app/owner)
- استخدام MS Graph -

    [المرجع: إضافة مالك - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- استخدام مدخل Azure AD - انتقل إلى portal.azure.com [>](https://portal.azure.com/) Azure Active directory > تسجيل التطبيقات > حدد تطبيقك > مالكو > إضافة مالكين

**هل يتعذر عليك عرض التطبيق على شفرة تسجيلات التطبيق على الرغم من أنك مالك هذا التطبيق؟**

لا يكون مالك التطبيق دورا إداريا. إذا تم تمكين الإعداد تقييد الوصول إلى مدخل إدارة [Azure AD،](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) سيكون المسؤول فقط قادرا على عرض التطبيقات على مدخل تسجيل التطبيق. لكي يتمكن المالك من عرض التطبيقات، قم إما بتعطيل هذا الإعداد (تعيين هذا الإعداد إلى لا) أو تعيين دور المسؤول إلى المالك للتطبيق المحدد فقط. على الرغم من ذلك، سوف تحتاج إلى ترخيص Azure AD Premium P2 وتمكين إدارة الهويات المتميزة [.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
