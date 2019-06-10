---
title: كيف-إلى--nk2-ملفات الاستيراد
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 1d1b02527c3b614375cf1f84a7a511d9318689b1
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770234"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="d5707-102">كيفية استيراد ملفات.nk2</span><span class="sxs-lookup"><span data-stu-id="d5707-102">How to import .nk2 files</span></span> 

<span data-ttu-id="d5707-103">عند بدء تشغيل Microsoft Outlook 2013، Outlook 2016 Outlook 2019 أو Outlook Office 365 للمرة الأولى، يتم استيراد الاسم المستعار ذاكرة التخزين المؤقت (المخزنة في ملف.nk2 *اسم ملف التعريف*) في رسالة مخفية في مخزن الرسائل الافتراضي الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="d5707-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="d5707-104">لاستيراد ملفات.nk2 إلى Outlook 2013 أو Outlook 2016 Outlook 2019 أو Outlook Office 365، تأكد من وجود الملف.nk2 في المجلد التالي: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="d5707-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="d5707-105">**ملاحظة**: يجب أن يكون لديك ملف.nk2 نفس اسم التشكيل الجانبي الحالي Outlook 2013 أو Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="d5707-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="d5707-106">يتم بشكل افتراضي، اسم ملف التعريف "Outlook".</span><span class="sxs-lookup"><span data-stu-id="d5707-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="d5707-107">للتحقق من اسم ملف التعريف، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="d5707-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="d5707-108">انقر فوق **ابدأ**، وفوق **لوحة التحكم**.</span><span class="sxs-lookup"><span data-stu-id="d5707-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="d5707-109">انقر نقراً مزدوجاً فوق **بريد**.</span><span class="sxs-lookup"><span data-stu-id="d5707-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="d5707-110">في مربع الحوار "إعداد البريد"، حدد **إظهار ملفات التعريف**.</span><span class="sxs-lookup"><span data-stu-id="d5707-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="d5707-111">حدد **تاريخ بدء** > **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="d5707-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="d5707-112">في المربع **فتح** ، اكتب *outlook.exe/importnk2*، ومن ثم حدد **"موافق"**.</span><span class="sxs-lookup"><span data-stu-id="d5707-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="d5707-113">بعد استيراد الملف.nk2، يتم دمج محتويات الملف في القائمة الكنيات تخزينها في علبة البريد الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="d5707-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="d5707-114">**ملاحظة**:.nk2 يتم إعادة تسمية الملف بملحق اسم ملف.old في المرة التالية التي تبدأ عام 2013 Outlook أو Outlook 2016 Outlook 2019 أو Outlook Office 365.</span><span class="sxs-lookup"><span data-stu-id="d5707-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365.</span></span> <span data-ttu-id="d5707-115">في حالة إعادة استيراد الملف.nk2، قم بإزالة ملحق اسم الملف.old أولاً.</span><span class="sxs-lookup"><span data-stu-id="d5707-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="d5707-116">لمزيد من المعلومات، راجع [استيراد أو نسخ قائمة "الإكمال التلقائي" إلى كمبيوتر آخر](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="d5707-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>