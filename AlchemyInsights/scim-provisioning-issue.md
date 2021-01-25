---
title: مشكله التزويد في سيم
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7854"
- "9004348"
ms.openlocfilehash: aa5b4cbb99cb1a5a323b39101766bea55fd49064
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949639"
---
# <a name="scim-provisioning-issue"></a><span data-ttu-id="e5f85-102">مشكله التزويد في سيم</span><span class="sxs-lookup"><span data-stu-id="e5f85-102">SCIM provisioning issue</span></span>

<span data-ttu-id="e5f85-103">يشير التوفير التلقائي إلى إنشاء هويات المستخدمين والأدوار في تطبيقات السحابة التي يحتاج المستخدمون إلى الوصول اليها.</span><span class="sxs-lookup"><span data-stu-id="e5f85-103">Automatic provisioning refers to creating user identities and roles in the cloud applications that users need access to.</span></span> <span data-ttu-id="e5f85-104">بالاضافه إلى إنشاء هويات المستخدمين ، يتضمن التوفير التلقائي الصيانة وأزاله هويات المستخدمين كتغيير في الحالة أو الأدوار.</span><span class="sxs-lookup"><span data-stu-id="e5f85-104">In addition to creating user identities, automatic provisioning includes the maintenance and removal of user identities as status or roles change.</span></span> <span data-ttu-id="e5f85-105">قبل ان تبدا عمليه نشر ، يمكنك مراجعه [كيفيه عمل التزويد](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) للتعرف علي كيفيه عمل Azure active DIRECTORY (AD) ، والحصول علي توصيات التكوين.</span><span class="sxs-lookup"><span data-stu-id="e5f85-105">Before you start a deployment, you can review [How provisioning works](https://docs.microsoft.com/azure/active-directory/app-provisioning/how-provisioning-works) to learn how Azure Active Directory (AD) provision works, and get configuration recommendations.</span></span>

<span data-ttu-id="e5f85-106">بصفتك مطور تطبيق ، يمكنك استخدام النظام لواجهه برمجه تطبيقات أداره الهوية عبر المجالات (سيم) لتمكين التوفير التلقائي للمستخدمين والمجموعات بين التطبيق و Azure AD.</span><span class="sxs-lookup"><span data-stu-id="e5f85-106">As an application developer, you can use the System for Cross-Domain Identity Management (SCIM) user management API to enable automatic provisioning of users and groups between your application and Azure AD.</span></span> <span data-ttu-id="e5f85-107">تصف [نقطه نهاية سيم وتكوين تزويد المستخدم باستخدام المقالة AZURE AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) كيفيه إنشاء نقطه نهاية سيم ودمجها باستخدام خدمه التزويد في Azure ad.</span><span class="sxs-lookup"><span data-stu-id="e5f85-107">The [Build a SCIM endpoint and configure user provisioning with Azure AD](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) article describes how to build an SCIM endpoint and integrate it with the Azure AD provisioning service.</span></span>



