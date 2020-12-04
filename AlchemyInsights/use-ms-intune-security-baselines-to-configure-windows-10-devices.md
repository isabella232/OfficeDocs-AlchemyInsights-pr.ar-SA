---
title: استخدام أساسات أمان Microsoft Intune لتكوين أجهزه Windows 10
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573268"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="5ddbc-102">استخدام أساسات أمان Microsoft Intune لتكوين أجهزه Windows 10</span><span class="sxs-lookup"><span data-stu-id="5ddbc-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="5ddbc-103">تساعد الخطوط الاساسيه للامان في Intune علي حماية المستخدمين والاجهزه.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="5ddbc-104">أساسات الأمان هي المجموعات التي تم تكوينها مسبقا في Windows لتطبيق مجموعه معروفه من الإعدادات والقيم الافتراضية الموصي بها بواسطة فرق الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="5ddbc-105">بإنشاء ملف تعريف أساس الأمان في Intune ، يمكنك إنشاء قالب يتكون من ملفات تعريف متعددة لتكوين الاجهزه.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="5ddbc-106">عند نشر أساسات الأمان علي مجموعات من المستخدمين أو الاجهزه ، يتم تطبيق الإعدادات علي الاجهزه التي يتم تشغيلها علي Windows 10 أو إصدار أحدث.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="5ddbc-107">علي سبيل المثال ، يقوم الأساس الخاص بأمان MDM تلقائيا (1) بتمكين BitLocker لمحركات الاقراص القابلة للازاله ، (2) يتطلب كلمه المرور الخاصة بإلغاء تامين جهاز ، و (3) بتعطيل المصادقة الاساسيه.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="5ddbc-108">عندما لا تعمل القيمة الافتراضية لبيئتك ، يمكنك تخصيص الأساس لتطبيق الإعدادات التي تحتاج اليها.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="5ddbc-109">تساعدك الخطوط الاساسيه أيضا في إنشاء سير عمل "متكامل الأمان" في Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="5ddbc-110">فيما يلي بعض المزايا التالية:</span><span class="sxs-lookup"><span data-stu-id="5ddbc-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="5ddbc-111">يتضمن أساس الأمان أفضل الممارسات والتوصيات لإعدادات تؤثر علي الأمان.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="5ddbc-112">نظرا لان شركاء Intune مع فريق أمان Windows الذين يقومون بإنشاء أساسات لنهج المجموعة ، فان هذه التوصيات تستند إلى الإرشادات المتصلة والتجربة الشاملة.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="5ddbc-113">إذا كنت جديدا في Intune ولم تكن متاكدا من مكان البدء ، سيساعدك أساس الأمان علي إنشاء ملف تعريف أمن ونشره بسرعة.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="5ddbc-114">إذا كنت تستخدم حاليا نهج مجموعه ، فمن الممكن ان تكون عمليه الترحيل إلى الغرض من الاداره ل Intune for management أكثر سهوله بالنسبة إلى أساسات الأمان ، لأنها مضمنه في Intune وتتضمن إمكانيات القص المتطورة للاداره.</span><span class="sxs-lookup"><span data-stu-id="5ddbc-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="5ddbc-115">لمعرفه المزيد ، راجع الخطوط الاساسيه [لامان Windows](https://go.microsoft.com/fwlink/?linkid=2141503) [وأداره الاجهزه المحمولة](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="5ddbc-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>