---
title: استخدام Microsoft Intune أساسيات الأمان لتكوين أجهزة Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793530"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="98f6e-102">استخدام Microsoft Intune أساسيات الأمان لتكوين أجهزة Windows 10</span><span class="sxs-lookup"><span data-stu-id="98f6e-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="98f6e-103">تساعد خطوط أمان Intune الأساسية على حماية المستخدمين والأجهزة.</span><span class="sxs-lookup"><span data-stu-id="98f6e-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="98f6e-104">إن خطوط الأمان الأساسية Windows الإعدادات التي تم تكوينها مسبقا وتستخدم لتطبيق مجموعة معروفة من الإعدادات والقيم الافتراضية الموصى بها من قبل فرق الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="98f6e-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="98f6e-105">من خلال إنشاء ملف تعريف أساسي أمان في Intune، يمكنك إنشاء قالب يتكون من ملفات تعريف تكوين أجهزة متعددة.</span><span class="sxs-lookup"><span data-stu-id="98f6e-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="98f6e-106">عند نشر خطوط الأمان الأساسية لمجموعات من المستخدمين أو الأجهزة، يتم تطبيق الإعدادات على الأجهزة التي يتم تشغيلها على Windows 10 أو لاحقا.</span><span class="sxs-lookup"><span data-stu-id="98f6e-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="98f6e-107">على سبيل المثال، يقوم أساسا أمان إدارة أجهزة Microsoft المحمولة (MDM) تلقائيا بتمكين BitLocker لمحركات الأقراص القابلة للإزالة، ويتطلب كلمة المرور لإلغاء تأمين جهاز، ويعطل المصادقة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="98f6e-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="98f6e-108">عندما لا تعمل قيمة افتراضية مع بيئتك، يمكنك تخصيص الأساس لتطبيق الإعدادات التي تحتاج إليها.</span><span class="sxs-lookup"><span data-stu-id="98f6e-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="98f6e-109">تساعد خطوط الأمان الأساسية أيضا على إنشاء سير عمل آمن من النهاية إلى النهاية في Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="98f6e-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="98f6e-110">يتضمن أساس الأمان أفضل الممارسات والتوصيات المتعلقة ب الإعدادات التي تؤثر على الأمان.</span><span class="sxs-lookup"><span data-stu-id="98f6e-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="98f6e-111">يقوم Intune بالشركاء Windows فريق الأمان الذي ينشئ خطوط أساسية لنهج المجموعة، لذا تستند هذه التوصيات إلى إرشادات قوية وتجربة واسعة النطاق.</span><span class="sxs-lookup"><span data-stu-id="98f6e-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="98f6e-112">إذا كنت جديدا في Intune وغير متأكد من مكان البدء، فإن خطوط الأمان الأساسية تساعدك على إنشاء ملف تعريف آمن ونشره بسرعة.</span><span class="sxs-lookup"><span data-stu-id="98f6e-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="98f6e-113">إذا كنت تستخدم حاليا نهج مجموعة، فإن عملية إجراء عملية إعادة التهجر إلى Intune لأغراض إدارية تكون أكثر سهولة مع خطوط الأمان الأساسية لأنها مضمنة في Intune وهي تتضمن قدرات الإدارة المتطورة.</span><span class="sxs-lookup"><span data-stu-id="98f6e-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="98f6e-114">لمعرفة المزيد، راجع Windows [أساسيات](/windows/security/threat-protection/windows-security-baselines) الأمان وإدارة [أجهزة المحمول](/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="98f6e-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

