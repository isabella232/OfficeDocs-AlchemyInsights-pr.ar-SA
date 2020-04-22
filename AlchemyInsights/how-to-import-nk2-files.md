---
title: كيف لاستيراد-nk2-الملفات
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 83d30b2d62908db791f21ec5ed7fd5537e7a0944
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759319"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="042b2-102">كيفية استيراد ملفات .nk2</span><span class="sxs-lookup"><span data-stu-id="042b2-102">How to import .nk2 files</span></span> 

<span data-ttu-id="042b2-103">عند بدء تشغيل Microsoft Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 للمرة الأولى، يتم استيراد ذاكرة التخزين المؤقت للكنية (المخزنة في ملف *اسم الملف الشخصي*.nk2) إلى رسالة مخفية في مخزن الرسائل الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="042b2-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="042b2-104">لاستيراد ملفات .nk2 إلى Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365، تأكد من أن ملف .nk2 موجود في المجلد التالي: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="042b2-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="042b2-105">**ملاحظة:** يجب أن يكون لملف .nk2 نفس اسم ملف Outlook 2013 الحالي أو ملف Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="042b2-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="042b2-106">بشكل افتراضي، اسم ملف التعريف هو "Outlook".</span><span class="sxs-lookup"><span data-stu-id="042b2-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="042b2-107">للتحقق من اسم الملف الشخصي، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="042b2-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="042b2-108">انقر فوق **ابدأ،** ثم انقر فوق **لوحة التحكم**.</span><span class="sxs-lookup"><span data-stu-id="042b2-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="042b2-109">انقر نقراً مزدوجاً على **البريد**.</span><span class="sxs-lookup"><span data-stu-id="042b2-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="042b2-110">في مربع حوار إعداد البريد، حدد **إظهار الملفات الشخصية**.</span><span class="sxs-lookup"><span data-stu-id="042b2-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="042b2-111">حدد **بدء** > **التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="042b2-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="042b2-112">في المربع **المفتوح،** اكتب *outlook.exe /importnk2،* ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="042b2-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="042b2-113">بعد استيراد ملف .nk2، يتم دمج محتويات الملف في ذاكرة التخزين المؤقت اللقب الموجودة المخزنة في علبة البريد الخاصة بك.</span><span class="sxs-lookup"><span data-stu-id="042b2-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="042b2-114">**ملاحظة:** تتم إعادة تسمية ملف .nk2 مع ملحق اسم ملف .old في المرة التالية التي تبدأ Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="042b2-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="042b2-115">إذا كنت ترغب في إعادة استيراد ملف .nk2، قم بإزالة ملحق اسم الملف القديم أولاً.</span><span class="sxs-lookup"><span data-stu-id="042b2-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="042b2-116">لمزيد من المعلومات، راجع [استيراد قائمة الإكمال التلقائي أو نسخها إلى كمبيوتر آخر](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="042b2-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>