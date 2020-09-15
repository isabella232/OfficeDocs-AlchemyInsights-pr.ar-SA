---
title: مفاتيح استرداد Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685873"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="74f3c-102">الوصول إلى مفاتيح استرداد Bitlocker</span><span class="sxs-lookup"><span data-stu-id="74f3c-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="74f3c-103">عند تكوين إعدادات Bitlocker لنهج حماية نقطه نهاية Intune ، يمكنك تحديد ما إذا كان يجب تخزين معلومات استرداد Bitlocker في Azure Active directory.</span><span class="sxs-lookup"><span data-stu-id="74f3c-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="74f3c-104">إذا تم تكوين هذا الاعداد ، فيجب ان تكون بيانات الاسترداد المخزنة مرئية لمسؤول Intune كجزء من البيانات الخاصة بسجل الجهاز في الريش الخاصة باجهزه Intune بطريقتين:</span><span class="sxs-lookup"><span data-stu-id="74f3c-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="74f3c-105">الاجهزه-أجهزه Azure AD-> "Device" أو الاجهزه-> كل الاجهزه-> "Device"-> مفاتيح الاسترداد</span><span class="sxs-lookup"><span data-stu-id="74f3c-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="74f3c-106">بدلا من ذلك ، إذا كان هناك حق الوصول الإداري إلى الجهاز نفسه ، فيمكنك الاطلاع علي مفتاح الاسترداد (كلمه المرور) عن طريق تشغيل الأمر التالي من موجه أوامر غير مقيد:</span><span class="sxs-lookup"><span data-stu-id="74f3c-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="74f3c-107">إذا تم تشفير الجهاز قبل الانرولمينت في Intune ، فمن المحتمل ان يكون قد تم اقران مفتاح الاسترداد ب "حساب Microsoft" (MSA) المستخدم لتسجيل الدخول إلى الجهاز اثناء عمليه OOBE.</span><span class="sxs-lookup"><span data-stu-id="74f3c-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="74f3c-108">إذا كانت هذه هي الحالة ،  https://onedrive.live.com/recoverykey سيعرض الوصول إلى الMSA وتسجيل الدخول باستخدام هذا النوع من الاجهزه التي تم تخزين مفاتيح الاسترداد الخاصة بها.</span><span class="sxs-lookup"><span data-stu-id="74f3c-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="74f3c-109">إذا تم تشفير الجهاز كنتيجة للتكوين عبر نهج المجموعة القائم علي المجال ، فمن المحتمل ان تكون معلومات الاسترداد مخزنه في Active Directory المحلي.</span><span class="sxs-lookup"><span data-stu-id="74f3c-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

