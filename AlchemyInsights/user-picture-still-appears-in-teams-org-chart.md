---
title: لا تزال صورة المستخدم تظهر في Microsoft Teams المؤسسة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2021
ms.locfileid: "59422178"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>لا تزال صورة المستخدم تظهر في Microsoft Teams المؤسسة

إذا تم تعطيل شخص واحد أو أكثر في مؤسستك أو إزالته، ولا تزال صورة ملف التعريف الخاصة به تظهر في المخطط المؤسسة، فمن المحتمل تعيين الإعداد **ShowInAddressLists** إلى False: 

1. انتقل إلى مركز مسؤولي Microsoft 365 > ["المستخدمون](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) النشطون" وحدد المستخدم الذي لا تزال الصورة تظهر فيه. 
1. حدد علامة **التبويب** البريد، وتأكد من تعيين إظهار في قائمة العنوان **العام** إلى **لا**.

إذا لم **ينجح تعيين ShowInAddressLists إلى** **لا،** فتحقق مما يلي: 

- قد يظهر المستخدم من قائمة المستلمين في Exchange. لمزيد من المعلومات، راجع [إدارة قوائم العنوان في Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- قد يظهر المستخدم من قائمة العنوان في Azure Active Directory. لمزيد من المعلومات، راجع [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 