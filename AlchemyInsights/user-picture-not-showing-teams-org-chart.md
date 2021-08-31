---
title: صورة المستخدم لا تظهر في Microsoft Teams المؤسسة
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 08/23/2021
ms.locfileid: "58792628"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>صورة المستخدم لا تظهر في Microsoft Teams المؤسسة

إذا فقد شخص واحد أو أكثر في مؤسستك صورة ملف التعريف الخاصة به في المخطط المؤسسة، فمن المحتمل تعيين الإعداد **ShowInAddressLists** إلى **False**:

1. انتقل إلى مركز مسؤولي Microsoft 365 > [**المستخدمون**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)النشطون ، وحدد المستخدم الذي تم فقدان الصورة له. 
1. حدد علامة **التبويب** البريد، وتأكد من تعيين إظهار في قائمة العنوان **العام** إلى **نعم**. 

إذا لم **ينجح تعيين ShowInAddressLists إلى** **نعم،** فتحقق مما يلي:

- قد يكون المستخدم مخفيا من قائمة المستلمين في Exchange. لمزيد من المعلومات، راجع [إدارة قوائم العنوان في Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- قد يكون المستخدم مخفيا من قائمة العنوان في Azure Active Directory. لمزيد من المعلومات، راجع [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 
