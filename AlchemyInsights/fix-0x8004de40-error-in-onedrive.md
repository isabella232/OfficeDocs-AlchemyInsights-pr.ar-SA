---
title: إصلاح 0x8004de40 في OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649735"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="bf43e-102">إصلاح 0x8004de40 في OneDrive</span><span class="sxs-lookup"><span data-stu-id="bf43e-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="bf43e-103">إذا كنت تقوم بتشغيل Windows 7 وتلقيت هذا الخطأ، فحدث لتمكين [TLS 1.1 و TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)كبروتوكولات آمنة افتراضية في WinHTTP في Windows .</span><span class="sxs-lookup"><span data-stu-id="bf43e-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="bf43e-104">إذا كنت تقوم بتشغيل Windows 10، وتلقيت رسالة خطأ 0x8004de40 OneDrive:</span><span class="sxs-lookup"><span data-stu-id="bf43e-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="bf43e-105">إعادة تشغيل الكمبيوتر المتأثر أثناء الاتصال بمجال Acitve Directory.</span><span class="sxs-lookup"><span data-stu-id="bf43e-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="bf43e-106">إذا لم تصلح عملية إعادة التشغيل المشكلة، ففك الانضمام إلى جهازك من Azure AD ثم إعادة الانضمام له.</span><span class="sxs-lookup"><span data-stu-id="bf43e-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="bf43e-107">**ملاحظة:** يجب أن تكون على شبكة الشركة أثناء تنفيذ هذه الخطوات.</span><span class="sxs-lookup"><span data-stu-id="bf43e-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="bf43e-108">لا تقوم بتنفيذ هذه الخطوات عندما لا تكون متصلا بالبنية الأساسية الخاصة بالشركة (على سبيل المثال، أثناء السفر).</span><span class="sxs-lookup"><span data-stu-id="bf43e-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="bf43e-109">افتح موجه أوامر غير مرفوط عن طريق تحديد **بدء،** وانقر ب زر الماوس الأيمن فوق **موجه الأوامر،** ثم حدد **تشغيل كمسؤول**.</span><span class="sxs-lookup"><span data-stu-id="bf43e-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="bf43e-110">اكتب *dsregcmd /leave واضغط* على **Enter**.</span><span class="sxs-lookup"><span data-stu-id="bf43e-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="bf43e-111">عند الإكمال، اكتب *dsregcmd /join واضغط* على **Enter**.</span><span class="sxs-lookup"><span data-stu-id="bf43e-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="bf43e-112">عند الانتهاء، أغلق موجه الأوامر.</span><span class="sxs-lookup"><span data-stu-id="bf43e-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="bf43e-113">إعادة تشغيل الكمبيوتر وتسجيل الدخول إلى OneDrive.</span><span class="sxs-lookup"><span data-stu-id="bf43e-113">Reboot the computer, and log into OneDrive.</span></span>