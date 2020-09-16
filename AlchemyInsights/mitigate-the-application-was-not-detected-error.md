---
title: الحد من حدوث خطأ عدم الكشف عن التطبيق
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666965"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="85970-102">الحد من حدوث خطأ "لم يتم الكشف عن التطبيق"</span><span class="sxs-lookup"><span data-stu-id="85970-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="85970-103">يحدث خطأ تثبيت التطبيق "لم يتم الكشف عن التطبيق بعد اكتمال التثبيت بنجاح"، والذي يتم الإبلاغ عنه بواسطة Intune، وقد يحدث في جميع أنظمة التشغيل الأساسية (Windows وiOS وAndroid).</span><span class="sxs-lookup"><span data-stu-id="85970-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="85970-104">السيناريوهات الأكثر شيوعاً التي تؤدي إلى حدوث هذا الخطأ:</span><span class="sxs-lookup"><span data-stu-id="85970-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="85970-105">تحديث التطبيق خارج Intune (من متجر تطبيقات تابع لجهة خارجية) بعد النشر الأولي.</span><span class="sxs-lookup"><span data-stu-id="85970-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="85970-106">على سبيل المثال، قد تقوم بعض التطبيقات مثل Google Chrome بإجراء تحديثات تلقائية.</span><span class="sxs-lookup"><span data-stu-id="85970-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="85970-107">قام أحد المستخدمين بإزالة تثبيت التطبيق بعد التثبيت الأولي.</span><span class="sxs-lookup"><span data-stu-id="85970-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="85970-108">للحد من هذه المشكلة، قم أولاً بمراجعة الأجهزة التي تأثرت لتحديد السيناريو الذي يحدث فيه الخطأ.</span><span class="sxs-lookup"><span data-stu-id="85970-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="85970-109">إذا تم تحديث التطبيق خارج Intune، يمكن تعيين نشر التطبيق بحيث يتجاهل إصدار التطبيق.</span><span class="sxs-lookup"><span data-stu-id="85970-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="85970-110">للقيام بذلك، ضمن **تكوين التطبيق > معلومات التطبيق**، قم بتعيين **تجاهل إصدار التطبيق** إلى **نعم**.</span><span class="sxs-lookup"><span data-stu-id="85970-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="85970-111">عند استهداف العميل، قد يكون من المناسب نشر التطبيق بوصفه "مطلوب"، والتأكد من نشر الإصدار الأخير.</span><span class="sxs-lookup"><span data-stu-id="85970-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="85970-112">بدلاً من ذلك، يمكن على النظام الأساسي iOS، استخدام وظيفة **التحديث التلقائي** المقترنة ببرنامج الشراء المجمع من Apple، والذي يمكن تكوينه ليتم التحديث تلقائياً إلى إصدارات التطبيق الحديثة بمجرد توفرها.</span><span class="sxs-lookup"><span data-stu-id="85970-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="85970-113">للحصول على المزيد من المعلومات حول استكشاف مشكلات تثبيت التطبيقات وإصلاحها، الرجاء مراجعة [استكشاف مشكلات تثبيت التطبيقات وإصلاحها](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="85970-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
