---
title: مفاهيم المصادقة المتقدمة المطبقة على Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398536"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="e7157-102">مفاهيم المصادقة المتقدمة المطبقة على Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e7157-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="e7157-103">فيما يلي مفاهيم المصادقة المتقدمة التي تنطبق على Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="e7157-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="e7157-104">**المصادقة الاستباقية**</span><span class="sxs-lookup"><span data-stu-id="e7157-104">**Proactive Authentication**</span></span>

<span data-ttu-id="e7157-105">عند تمكين نهج [ProactiveAuthEnabled،](https://go.microsoft.com/fwlink/?linkid=2134621) سيحاول Microsoft Edge المصادقة بشكل استباقي على المستخدمين الذين تم توقيعهم من خلال خدمات Microsoft.</span><span class="sxs-lookup"><span data-stu-id="e7157-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="e7157-106">في فواصل زمنية منتظمة، سيستخدم خدمة عبر الإنترنت للتحقق من وجود بيان محدث يحتوي على التكوين الذي يحكم المصادقة الاستباقية.</span><span class="sxs-lookup"><span data-stu-id="e7157-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="e7157-107">الفوائد: تمكن المصادقة الاستباقية المصادقة للخدمات الأساسية، مثل صفحة علامة تبويب Office الجديدة.</span><span class="sxs-lookup"><span data-stu-id="e7157-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="e7157-108">بالإضافة إلى ذلك، إذا تم استخدام Bing كمحرك بحث، فإن المصادقة الاستباقية تحسن أداء شريط العنوان وتساعد على إنشاء نتائج بحث مخصصة لتلبية احتياجات عملك.</span><span class="sxs-lookup"><span data-stu-id="e7157-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="e7157-109">**Windows Hello CredUI لمصادقة NTLM**</span><span class="sxs-lookup"><span data-stu-id="e7157-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="e7157-110">إذا لم يكن تسجيل الدخول الفردي (SSO) متوفرا عندما يحاول موقع ويب تسجيل الدخول إلى المستخدم من خلال الآلية NTLM أو التفاوض، فإن هذه الميزة ستسمح للمستخدم بمشاركة بيانات اعتماد نظام التشغيل مع موقع ويب وتلبية تحدي المصادقة باستخدام واجهة مستخدم Windows Hello Cred.</span><span class="sxs-lookup"><span data-stu-id="e7157-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="e7157-111">سيظهر تدفق تسجيل الدخول هذا فقط في Windows 10 فقط للمستخدمين الذين لم ينتهوا من تسجيل الدخول خلال NTLM أو في تحدي التفاوض.</span><span class="sxs-lookup"><span data-stu-id="e7157-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="e7157-112">**استخدام كلمات المرور المحفوظة في تسجيل الدخول تلقائيا**</span><span class="sxs-lookup"><span data-stu-id="e7157-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="e7157-113">يمكن للمستخدمين الذين يحفظون كلمات المرور في Microsoft Edge تمكين تسجيل الدخول التلقائي إلى مواقع الويب حيث تم حفظ بيانات الاعتماد.</span><span class="sxs-lookup"><span data-stu-id="e7157-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="e7157-114">يمكن للمستخدمين تشغيل هذه الميزة أو إيقاف تشغيلها في edge://settings/passwords، كما يمكنك تكوينها في سياسات [إدارة كلمات](https://go.microsoft.com/fwlink/?linkid=2134622) المرور.</span><span class="sxs-lookup"><span data-stu-id="e7157-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
