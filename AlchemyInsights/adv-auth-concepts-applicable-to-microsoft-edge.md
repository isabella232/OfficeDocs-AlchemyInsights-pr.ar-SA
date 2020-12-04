---
title: مفاهيم المصادقة المتقدمة المطبقة علي Microsoft Edge
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
ms.openlocfilehash: 241d594fac6664dd1e85fd60e30a6344c432555e
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573267"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a><span data-ttu-id="90fe6-102">مفاهيم المصادقة المتقدمة المطبقة علي Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="90fe6-102">Advanced authentication concepts applicable to Microsoft Edge</span></span>

<span data-ttu-id="90fe6-103">فيما يلي مفاهيم المصادقة المتقدمة التي تنطبق علي Microsoft Edge:</span><span class="sxs-lookup"><span data-stu-id="90fe6-103">Following are the advanced authentication concepts that are applicable to Microsoft Edge:</span></span>

<span data-ttu-id="90fe6-104">**المصادقة الاستباقية**</span><span class="sxs-lookup"><span data-stu-id="90fe6-104">**Proactive Authentication**</span></span>

<span data-ttu-id="90fe6-105">عند تمكين نهج [برواكتيفيوثينابليد](https://go.microsoft.com/fwlink/?linkid=2134621) ، سيحاول Microsoft Edge مصادقه المستخدمين الذين تم تسجيل دخولهم بفاعليه عبر خدمات Microsoft.</span><span class="sxs-lookup"><span data-stu-id="90fe6-105">When you enable the [ProactiveAuthEnabled](https://go.microsoft.com/fwlink/?linkid=2134621) policy, Microsoft Edge will try to proactively authenticate signed-in users through Microsoft services.</span></span> <span data-ttu-id="90fe6-106">عند الفواصل الزمنيه المنتظمة ، ستستخدم خدمه عبر الإنترنت للتحقق من البيانات المحدثة التي تحتوي علي المصادقة الاستباقية لتحكم التكوين.</span><span class="sxs-lookup"><span data-stu-id="90fe6-106">At regular intervals, it will use an online service to check for an updated manifest that contains the configuration governing Proactive Authentication.</span></span>

<span data-ttu-id="90fe6-107">الفوائد: تمكن المصادقة الاستباقية المصادقة علي الخدمات الاساسيه ، مثل صفحه علامة التبويب الجديدة في Office.</span><span class="sxs-lookup"><span data-stu-id="90fe6-107">Benefits: Proactive Authentication enables authentication to key services, such as the Office New Tab Page.</span></span> <span data-ttu-id="90fe6-108">بالاضافه إلى ذلك ، إذا تم استخدام Bing كمحرك بحث ، فان المصادقة الاستباقية تحسن أداء شريط العناوين ويساعد علي إنشاء نتائج البحث المخصصة لاحتياجات شركتك.</span><span class="sxs-lookup"><span data-stu-id="90fe6-108">Also, if Bing is used as the search engine, Proactive Authentication improves the performance of the address bar and helps generate search results personalized to the needs of your business.</span></span>

<span data-ttu-id="90fe6-109">**كريدوي Windows Hello لمصادقه NTLM**</span><span class="sxs-lookup"><span data-stu-id="90fe6-109">**Windows Hello CredUI for NTLM Authentication**</span></span>

<span data-ttu-id="90fe6-110">إذا لم تكن ميزه تسجيل الدخول الأحادي (SSO) متوفرة عندما يحاول موقع ويب تسجيل الدخول علي المستخدم من خلال اليه NTLM أو التفاوض ، ستسمح هذه الخاصية للمستخدم بمشاركه بيانات اعتماد نظام التشغيل باستخدام موقع ويب ولتلبيه ارتياب المصادقة بواسطة واجهه مستخدم بيانات الاعتماد الخاصة ب Windows Hello.</span><span class="sxs-lookup"><span data-stu-id="90fe6-110">If single sign-on (SSO) isn't available when a website tries to sign on the user through the NTLM or Negotiate mechanism, this feature will allow the user to share the OS credentials with the website and to satisfy the authentication challenge by using Windows Hello Cred UI.</span></span> <span data-ttu-id="90fe6-111">سيظهر تدفق تسجيل الدخول هذا فقط في Windows 10 وللمستخدمين الذين لا يمكنهم الحصول علي SSO خلال NTLM أو تحدي في التفاوض.</span><span class="sxs-lookup"><span data-stu-id="90fe6-111">This sign-on flow will appear only in Windows 10 and only for users who don't get SSO during an NTLM or a Negotiate challenge.</span></span>

<span data-ttu-id="90fe6-112">**استخدام كلمات المرور المحفوظة لتسجيل الدخول تلقائيا**</span><span class="sxs-lookup"><span data-stu-id="90fe6-112">**Use saved passwords to sign on automatically**</span></span>

<span data-ttu-id="90fe6-113">يمكن للمستخدمين الذين يحفظون كلمات المرور في Microsoft Edge تمكين تسجيل الدخول التلقائي إلى مواقع الويب التي قاموا بحفظ بيانات الاعتماد بها.</span><span class="sxs-lookup"><span data-stu-id="90fe6-113">Users who save passwords in Microsoft Edge can enable automatic sign-on to websites where they have saved credentials.</span></span> <span data-ttu-id="90fe6-114">يمكن للمستخدمين تشغيل هذه الميزة أو إيقاف تشغيلها في edge://settings/passwords ، ويمكنك تكوينها في نهج [أداره كلمه المرور](https://go.microsoft.com/fwlink/?linkid=2134622) .</span><span class="sxs-lookup"><span data-stu-id="90fe6-114">Users can turn this feature on or off in edge://settings/passwords, and you can configure it in the [password manager](https://go.microsoft.com/fwlink/?linkid=2134622) policies.</span></span>
