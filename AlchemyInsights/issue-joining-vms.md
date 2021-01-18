---
title: الانضمام إلى VMs
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884804"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="f3258-102">الانضمام إلى VMs</span><span class="sxs-lookup"><span data-stu-id="f3258-102">Issue joining VMs</span></span>

<span data-ttu-id="f3258-103">لحل المشاكل التي تحدث اثناء محاولة الانضمام إلى VMs ، نفذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="f3258-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="f3258-104">حاول تسجيل الدخول باستخدام تنسيق **UPN** (علي سبيل المثال ، ' joeuser@contoso.com ') بدلا من تنسيق **ساماككونتنامي** (' contoso\joeuser ').</span><span class="sxs-lookup"><span data-stu-id="f3258-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="f3258-105">تاكد من انك قمت بتمكين مزامنة كلمه المرور بالتوافق مع الخطوات المذكورة في دليل *بدء* الاستخدام.</span><span class="sxs-lookup"><span data-stu-id="f3258-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="f3258-106">تاكد من ان حساب المستخدم المتاثر ليس حسابا خارجيا في مستاجر Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3258-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="f3258-107">لا يمكن للمستخدمين الخارجيين تسجيل الدخول إلى المجال المدار بما ان خدمات مجال Azure AD لا تملك بيانات اعتماد لحسابات المستخدمين هذه.</span><span class="sxs-lookup"><span data-stu-id="f3258-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="f3258-108">إذا كان حساب المستخدم المتاثر هو حساب مستخدم خاص بالسحابة ، فتاكد من قيام المستخدمين بتغيير كلمه المرور الخاصة بهم بعد تمكين خدمات مجالات Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3258-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="f3258-109">تؤدي هذه الخطوة إلى إنشاء تجزئات بيانات الاعتماد المطلوبة لخدمات مجال Azure AD.</span><span class="sxs-lookup"><span data-stu-id="f3258-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="f3258-110">إذا تمت مزامنة حسابات المستخدمين المتاثرين من دليل محلي ، فتاكد من تكوين الإصدار الموصي به من Azure AD Connect لاجراء مزامنة كامله.</span><span class="sxs-lookup"><span data-stu-id="f3258-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="f3258-111">إذا استمرت المشاكل بعد تاكيد الخطوة 4 ، فقم بتنفيذ الأوامر التالية من جهاز المزامنة:</span><span class="sxs-lookup"><span data-stu-id="f3258-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="f3258-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="f3258-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>