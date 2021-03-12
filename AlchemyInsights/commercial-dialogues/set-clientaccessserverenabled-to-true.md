---
title: تعيين ClientAccessServerEnabled إلى True
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50743153"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="42ab7-102">تعيين ClientAccessServerEnabled إلى True</span><span class="sxs-lookup"><span data-stu-id="42ab7-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="42ab7-103">إذا لم تتمكن من فتح رسالة بريد إلكتروني مشفرة وبدلا من ذلك رأيت مرفق **rpmsg،** فتابع تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="42ab7-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="42ab7-104">الاتصال ب Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="42ab7-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="42ab7-105">للاتصال ب Exchange Online PowerShell، يجب تسجيل الدخول باستخدام مسؤول عام أو حساب مسؤول Exchange.</span><span class="sxs-lookup"><span data-stu-id="42ab7-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="42ab7-106">أ.</span><span class="sxs-lookup"><span data-stu-id="42ab7-106">a.</span></span> <span data-ttu-id="42ab7-107">افتح Windows PowerShell، ثم قم بتشغيل الأمر التالي: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="42ab7-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="42ab7-108">ب.</span><span class="sxs-lookup"><span data-stu-id="42ab7-108">b.</span></span> <span data-ttu-id="42ab7-109">في مربع الحوار طلب اعتماد **Windows PowerShell،** أدخل حساب العمل أو المدرسة وكلمة المرور، ج.</span><span class="sxs-lookup"><span data-stu-id="42ab7-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="42ab7-110">انقر فوق **موافق**.</span><span class="sxs-lookup"><span data-stu-id="42ab7-110">Click **OK**.</span></span> 

2. <span data-ttu-id="42ab7-111">قم بتشغيل الأمر التالي لإنشاء جلسة عمل جديدة:</span><span class="sxs-lookup"><span data-stu-id="42ab7-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="42ab7-112">أ.</span><span class="sxs-lookup"><span data-stu-id="42ab7-112">a.</span></span> <span data-ttu-id="42ab7-113">قم بتنفيذ الأمر التالي:</span><span class="sxs-lookup"><span data-stu-id="42ab7-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="42ab7-114">الأمر `Get-IRMConfiguration` "تشغيل".</span><span class="sxs-lookup"><span data-stu-id="42ab7-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="42ab7-115">تحقق من **الإعداد ClientAccessServerEnabled.**</span><span class="sxs-lookup"><span data-stu-id="42ab7-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="42ab7-116">أ.</span><span class="sxs-lookup"><span data-stu-id="42ab7-116">a.</span></span> <span data-ttu-id="42ab7-117">إذا **تم تعيين إعداد ClientAccessServerEnabled** إلى **False**، ف قم بتشغيل أمر cmdlet التالي: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="42ab7-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="42ab7-118">أغلق جلسة powershell دائما باستخدام الأمر التالي: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="42ab7-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="42ab7-119">لمزيد من المعلومات، راجع [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="42ab7-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

