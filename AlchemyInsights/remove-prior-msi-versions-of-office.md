---
title: أزاله إصدارات MSI السابقة من Office
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680643"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="53103-102">أزاله إصدارات MSI السابقة من Office</span><span class="sxs-lookup"><span data-stu-id="53103-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="53103-103">نوصي بازاله الإصدارات السابقة من Windows Installer (MSI) من Office قبل تثبيت Office 365 ProPlus.</span><span class="sxs-lookup"><span data-stu-id="53103-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="53103-104">اليك كيفيه القيام بذلك:</span><span class="sxs-lookup"><span data-stu-id="53103-104">Here's how to do this:</span></span>

1. <span data-ttu-id="53103-105">إذا استخدمت MSI لتثبيت Office ، فيمكنك استخدام أداه نشر Office (ODT) لأزاله تثبيت Office.</span><span class="sxs-lookup"><span data-stu-id="53103-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="53103-106">يمكنك استخدام عنصر ريموفيمسي في ملف **configuration.xml** الخاص بك.</span><span class="sxs-lookup"><span data-stu-id="53103-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="53103-107">اتبع الإرشادات الموجودة في هذه المقالة: [أمان Office 365 & مركز التوافق.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span><span class="sxs-lookup"><span data-stu-id="53103-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>