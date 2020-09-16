---
title: مركز مسؤولي Teams
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
- "9002890"
- "5542"
ms.openlocfilehash: bb0d757aab05132ff7169ce75009d7012b9a836c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670351"
---
# <a name="teams-admin-center"></a><span data-ttu-id="bfa52-102">مركز مسؤولي Teams</span><span class="sxs-lookup"><span data-stu-id="bfa52-102">Teams Admin Center</span></span>

<span data-ttu-id="bfa52-103">تعرّف على ماهية الإدارة في Teams مع [مركز مسؤولي Teams](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="bfa52-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="bfa52-104">إذا لم تكن قادراً على الوصول إلى مركز مسؤولي Teams، فالرجاء التحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="bfa52-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="bfa52-105">تحقق من أنك قمت بالسماح [بعناوين IP وURL المناسبة لـ Office 365](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) على أجهزة المراقبة (جدار الحماية وغير ذلك) أو قواعد جدار الحماية على جهازك المحلي.</span><span class="sxs-lookup"><span data-stu-id="bfa52-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="bfa52-106">تحقق من أن معلومات تسجيل الدخول التي تستخدمها للوصول إلى مدخل مسؤولي Teams متطابقة مع اسم المستخدم المدرج في [مدخل مسؤولي Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="bfa52-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="bfa52-107">إذا لم يظهر المستخدمون في مركز مسؤولي Teams، فالرجاء التحقق مما يلي:</span><span class="sxs-lookup"><span data-stu-id="bfa52-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="bfa52-108">هل قمت بإنشاء مستخدمين أو بتعيين تراخيص خلال 24 ساعة السابقة؟</span><span class="sxs-lookup"><span data-stu-id="bfa52-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="bfa52-109">قبل فتح تذكرة الدعم، الرجاء الانتظار لمدة 24 ساعة على الأقل.</span><span class="sxs-lookup"><span data-stu-id="bfa52-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="bfa52-110">هل تريد التحقق من أنك قمت بتعيين التراخيص المناسبة؟</span><span class="sxs-lookup"><span data-stu-id="bfa52-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="bfa52-111">إذا كان لديك Active Directory محلي ، فتحقق من ان [قيمه مسرتكسيب بريماريوسيرادريس أو عنوان SIP في الحقل ProxyAddresses في الدليل المحلي Active directory فريد وتطابق التنسيق](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) SIP:**اسم** المستخدم من مركز أداره الخاص ب [Microsoft 365](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span><span class="sxs-lookup"><span data-stu-id="bfa52-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="bfa52-112">إذا كنت ترغب في الاحتفاظ بنشر خادم Skype for Business وكان لدي المستخدمين يستخدم محليا ومتصلا بالإنترنت: اتبع **"اعداد المختلط باستخدام الفرق و Skype For Business Online"** في لوحه تحكم Skype For business Server ونقل المستخدمين عبر الإنترنت.</span><span class="sxs-lookup"><span data-stu-id="bfa52-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
