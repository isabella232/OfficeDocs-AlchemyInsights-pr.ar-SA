---
title: استخدام خطوط أمان Microsoft Intune لتكوين أجهزة Windows 10
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50692650"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="b93fd-102">استخدام خطوط أمان Microsoft Intune لتكوين أجهزة Windows 10</span><span class="sxs-lookup"><span data-stu-id="b93fd-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="b93fd-103">تساعد خطوط أمان Intune الأساسية على حماية المستخدمين والأجهزة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="b93fd-104">إن خطوط الأمان الأساسية هي مجموعات إعدادات Windows التي تم تكوينها مسبقا وتستخدم لتطبيق مجموعة معروفة من الإعدادات والقيم الافتراضية الموصى بها من قبل فرق الأمان ذات الصلة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="b93fd-105">من خلال إنشاء ملف تعريف أساسي أمان في Intune، يمكنك إنشاء قالب يتكون من ملفات تعريف تكوين جهاز متعددة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="b93fd-106">عند نشر خطوط الأمان الأساسية لمجموعات من المستخدمين أو الأجهزة، يتم تطبيق الإعدادات على الأجهزة التي يتم تشغيلها على Windows 10 أو الإصدارات الأحدث.</span><span class="sxs-lookup"><span data-stu-id="b93fd-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="b93fd-107">على سبيل المثال، يقوم أساس أمان إدارة أجهزة المحمول (MDM) من Microsoft تلقائيا (1) بتمكين BitLocker لمحركات الأقراص القابلة للإزالة، و(2) يتطلب كلمة المرور لإلغاء تأمين جهاز، و(3) تعطيل المصادقة الأساسية.</span><span class="sxs-lookup"><span data-stu-id="b93fd-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="b93fd-108">عندما لا تعمل قيمة افتراضية مع بيئتك، يمكنك تخصيص الأساس لتطبيق الإعدادات التي تحتاجها.</span><span class="sxs-lookup"><span data-stu-id="b93fd-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="b93fd-109">تساعد خطوط الأمان الأساسية أيضا على إنشاء سير عمل آمن بشكل منته في Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b93fd-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="b93fd-110">فيما يلي بعض فوائد هذه الوظيفة:</span><span class="sxs-lookup"><span data-stu-id="b93fd-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="b93fd-111">يتضمن أساس الأمان أفضل الممارسات والتوصيات المتعلقة ب الإعدادات التي تؤثر على الأمان.</span><span class="sxs-lookup"><span data-stu-id="b93fd-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="b93fd-112">نظرا لأن Intune يعمل مع فريق أمان Windows الذي يقوم بإنشاء خطوط أساسية لنهج المجموعة، فإن هذه التوصيات تستند إلى إرشادات قوية وتجربة واسعة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="b93fd-113">إذا لم يكن Intune جديدا بالنسبة لك وغير متأكد من المكان الذي تريد البدء منه، فإن خطوط الأمان الأساسية ستساعدك على إنشاء ملف تعريف آمن ونشره بسرعة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="b93fd-114">إذا كنت تستخدم حاليا نهج مجموعة، فإن عملية التهجر إلى Intune لأغراض الإدارة تكون أكثر سهولة مع خطوط الأمان الأساسية، لأن خطوط الأمان الأساسية هذه مضمنة في Intune وتتضمن قدرات الإدارة المتطورة.</span><span class="sxs-lookup"><span data-stu-id="b93fd-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="b93fd-115">لمزيد من المعلومات، راجع خطوط [أمان Windows وإدارة](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) أجهزة [المحمول.](https://docs.microsoft.com/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="b93fd-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>