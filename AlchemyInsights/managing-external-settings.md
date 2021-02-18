---
title: إدارة الإعدادات الخارجية
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8322"
- "9003227"
ms.openlocfilehash: 7caf46f9988ddbcbb16c0a2751dbda85bd7da34c
ms.sourcegitcommit: 616ae0cbd5769e12ae428e00088840cf05e52b6a
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 02/17/2021
ms.locfileid: "50294127"
---
# <a name="managing-external-settings"></a><span data-ttu-id="40e53-102">إدارة الإعدادات الخارجية</span><span class="sxs-lookup"><span data-stu-id="40e53-102">Managing External Settings</span></span>

<span data-ttu-id="40e53-103">**إعلان**</span><span class="sxs-lookup"><span data-stu-id="40e53-103">**Announcement**</span></span>

- <span data-ttu-id="40e53-104">إهمال دعم تسجيل الدخول إلى WebView من Google بدءا من [4 يناير 2021.](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="40e53-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](https://docs.microsoft.com/azure/active-directory/external-identities/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support#deprecation-of-webview-sign-in-support).</span></span> <span data-ttu-id="40e53-105">اختبار ما إذا كانت تطبيقاتك تتأثر باتباع إرشادات Google حول اختبار التوافق</span><span class="sxs-lookup"><span data-stu-id="40e53-105">Test whether your apps are affected by following Google’s guidance on testing compatibility</span></span>
- <span data-ttu-id="40e53-106">تأكد من استخدام عرض ويب النظام أو مستعرض النظام عند تسجيل الدخول إلى المستخدمين باستخدام حسابات Google للمستهلكين</span><span class="sxs-lookup"><span data-stu-id="40e53-106">Make sure to use the system webview or the system browser when signing in your users with consumer Google accounts</span></span>

<span data-ttu-id="40e53-107">**إدارة إعدادات الدعوة**</span><span class="sxs-lookup"><span data-stu-id="40e53-107">**Manage Invitation Settings**</span></span>

<span data-ttu-id="40e53-108">تأكد من تكوين إعدادات التعاون [الخارجي](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) للسماح للأشخاص المناسبين بإرسال الدعوات.</span><span class="sxs-lookup"><span data-stu-id="40e53-108">Confirm that you have [configured the external collaboration settings](https://docs.microsoft.com/azure/active-directory/external-identities/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support) to allow the appropriate people to send invitations.</span></span>

<span data-ttu-id="40e53-109">**إدارة أذونات وصول المستخدم الضيف**</span><span class="sxs-lookup"><span data-stu-id="40e53-109">**Manage Guest User Access Permissions**</span></span>

1. <span data-ttu-id="40e53-110">يمكن للمسؤولين العامين إدارة أذونات وصول الضيوف في الدليل من خلال مدخل Azure من خلال تكوين أذونات وصول الضيف على الصفحة "إعدادات التعاون الخارجي".</span><span class="sxs-lookup"><span data-stu-id="40e53-110">Global admins can manage guest access permissions in the directory through the Azure portal by configuring the guest access permissions on the External Collaboration Settings page.</span></span> <span data-ttu-id="40e53-111">[تعرف على المزيد حول هذا الإعداد.](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="40e53-111">[Learn more about this setting](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
2. <span data-ttu-id="40e53-112">إذا كنت ترغب في وصول الضيوف إلى تطبيقات مثل Teams أو SharePoint، فتأكد من أنك قمت بتكوين هذه التطبيقات للسماح بو وصول الضيف.</span><span class="sxs-lookup"><span data-stu-id="40e53-112">If you would like your guests to access apps such as Teams or SharePoint, confirm that you've configured those apps to allow guest access.</span></span> <span data-ttu-id="40e53-113">تعرف على المزيد حول [إعدادات Teams](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) [و SharePoint.](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="40e53-113">Learn more about the [Teams settings](https://docs.microsoft.com/microsoftteams/guest-access?WT.mc_id=Portal-Microsoft_Azure_Support) and [SharePoint](https://docs.microsoft.com/sharepoint/external-sharing-overview?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="40e53-114">**تكوين الدعوات:**</span><span class="sxs-lookup"><span data-stu-id="40e53-114">**Configuring invitations:**</span></span>

- [<span data-ttu-id="40e53-115">تمكين التعاون الخارجي B2B وإدارة الأشخاص الذين يمكنهم دعوة الضيوف</span><span class="sxs-lookup"><span data-stu-id="40e53-115">Enable B2B external collaboration and manage who can invite guests</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/delegate-invitations?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="40e53-116">السماح بالدعوات أو حظرها لمستخدمين من مؤسسات معينة</span><span class="sxs-lookup"><span data-stu-id="40e53-116">Allow or block invitations to users from specific organizations</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/allow-deny-list?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="40e53-117">**تكوين موفري الهويات المسموح لهم:**</span><span class="sxs-lookup"><span data-stu-id="40e53-117">**Configuring allowed identity providers:**</span></span>

- [<span data-ttu-id="40e53-118">Google Federation</span><span class="sxs-lookup"><span data-stu-id="40e53-118">Google Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/google-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="40e53-119">الاتحاد المباشر</span><span class="sxs-lookup"><span data-stu-id="40e53-119">Direct Federation</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/direct-federation?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="40e53-120">إرسال مصادقة رمز المرور عبر البريد الإلكتروني مرة واحدة</span><span class="sxs-lookup"><span data-stu-id="40e53-120">Email one-time Passcode Authentication</span></span>](https://docs.microsoft.com/azure/active-directory/b2b/one-time-passcode?WT.mc_id=Portal-Microsoft_Azure_Support)
