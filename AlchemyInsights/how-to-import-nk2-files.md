---
title: كيفيه الاستيراد-nk2 الملفات
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 6a823f6e0c4c46de64dd7b70fb40c76255d78ec1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780046"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="24060-102">كيفيه استيراد ملفات nk2</span><span class="sxs-lookup"><span data-stu-id="24060-102">How to import .nk2 files</span></span> 

<span data-ttu-id="24060-103">عند بدء تشغيل Microsoft Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 للمرة الاولي ، يتم استيراد ذاكره التخزين المؤقت لكنية (المخزنة في الملف *profilename*nk2) إلى رسالة مخفيه في مخزن الرسائل الافتراضي.</span><span class="sxs-lookup"><span data-stu-id="24060-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="24060-104">لاستيراد ملفات nk2 إلى Outlook 2013 أو Outlook 2016 أو Outlook 2019 أو Outlook for Microsoft 365 ، تاكد من ان ملف nk2 موجود في المجلد التالي:%appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="24060-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="24060-105">**ملاحظه**: يجب ان يكون لملف nk2 اسم ملف تعريف outlook 2013 أو outlook 2016 الحالي.</span><span class="sxs-lookup"><span data-stu-id="24060-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="24060-106">بشكل افتراضي ، يكون اسم التشكيل الجانبي هو "Outlook."</span><span class="sxs-lookup"><span data-stu-id="24060-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="24060-107">للتحقق من اسم ملف التعريف ، اتبع الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="24060-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="24060-108">انقر فوق **أبدا**، ثم فوق **لوحه التحكم**.</span><span class="sxs-lookup"><span data-stu-id="24060-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="24060-109">انقر نقرا مزدوجا فوق **البريد**.</span><span class="sxs-lookup"><span data-stu-id="24060-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="24060-110">في مربع الحوار اعداد البريد ، حدد **إظهار ملفات التعريف**.</span><span class="sxs-lookup"><span data-stu-id="24060-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="24060-111">حدد **بدء**  >  **التشغيل**.</span><span class="sxs-lookup"><span data-stu-id="24060-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="24060-112">في المربع **فتح** ، اكتب *outlook.exe/importnk2*، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="24060-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="24060-113">بعد استيراد الملف nk2 ، يتم دمج محتويات الملف في ذاكره التخزين المؤقت لكنية الموجودة المخزنة في علبه البريد.</span><span class="sxs-lookup"><span data-stu-id="24060-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="24060-114">**ملاحظه**: يتم أعاده تسميه ملف nk2 باستخدام ملحق اسم الملف القديم في المرة التالية التي تقوم فيها بتشغيل outlook 2013 أو outlook 2016 أو outlook 2019 أو Outlook ل Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="24060-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Microsoft 365.</span></span> <span data-ttu-id="24060-115">إذا أردت أعاده استيراد ملف nk2 ، فقم بازاله ملحق اسم الملف القديم أولا.</span><span class="sxs-lookup"><span data-stu-id="24060-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="24060-116">لمزيد من المعلومات ، راجع [استيراد قائمه الإكمال التلقائي أو نسخها إلى كمبيوتر آخر](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="24060-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>