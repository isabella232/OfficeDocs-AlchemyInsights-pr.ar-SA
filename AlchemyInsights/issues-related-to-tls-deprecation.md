---
title: تعذر إرسال/تلقي البريد الإلكتروني إلى/من Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50742933"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="9c8e6-102">تعذر إرسال/تلقي البريد الإلكتروني إلى/من Office 365 بسبب تعطيل TLS 1.0 و TLS 1.1</span><span class="sxs-lookup"><span data-stu-id="9c8e6-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="9c8e6-103">كما تم التأكيد من خلال نشر مركز الرسائل MC229914، بدأ إهمال TLS 1.0 و TLS 1.1 بفرض نقاط نهاية تدفق بريد Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="9c8e6-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="9c8e6-104">قريبا لن يقبل Office 365 اتصالات البريد الإلكتروني TLS 1.0 و TLS 1.1 من المصادر الخارجية.</span><span class="sxs-lookup"><span data-stu-id="9c8e6-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="9c8e6-105">كما لن يستخدم Exchange Online أبدا TLS 1.0 أو 1.1 لإرسال البريد الإلكتروني الصادر.</span><span class="sxs-lookup"><span data-stu-id="9c8e6-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="9c8e6-106">إذا كنت تواجه مشاكل بسبب تعطيل TLS 1.0 أو 1.1، فقد تواجه أحد الأخطاء التالية-</span><span class="sxs-lookup"><span data-stu-id="9c8e6-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="9c8e6-107">المرسل يسترد رسائل البريد المرتد ل NDR - '421 4.4.2 تم إسقاط الاتصال بسبب SocketError'</span><span class="sxs-lookup"><span data-stu-id="9c8e6-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="9c8e6-108">خطأ في "عارض قائمة الانتظار" للخادم "المحلية" الذي يرسل بريدا إلكترونيا إلى المسؤول 365- "تم إسقاط اتصال 421 4.4.2 بسبب "مأخذ التوصيل"</span><span class="sxs-lookup"><span data-stu-id="9c8e6-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="9c8e6-109">خطأ في إرسال سجل بروتوكول [الموصل](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) على الخادم الذي يرسل بريدا إلكترونيا إلى Office 365- فشل التفاوض بشأن TLS مع خطأ SocketError</span><span class="sxs-lookup"><span data-stu-id="9c8e6-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="9c8e6-110">خطأ في إرسال سجل بروتوكول الموصل أو تلقيه - '451 5.7.3 يجب أن يتم إصدار أمر STARTTLS أولا'</span><span class="sxs-lookup"><span data-stu-id="9c8e6-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="9c8e6-111">إذا واجهت أي من الأخطاء أعلاه، فالرجاء التأكد من تمكين TLS 1.2 على الخادم الذي يرسل بريدا إلكترونيا أو يتلقى البريد الإلكتروني من خلال التحقق من مفاتيح التسجيل التالية-</span><span class="sxs-lookup"><span data-stu-id="9c8e6-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="9c8e6-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:000000000 "Enabled"=dword:00000001**</span><span class="sxs-lookup"><span data-stu-id="9c8e6-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="9c8e6-113">إذا قمت بإجراء أي تغيير في مفاتيح التسجيل أعلاه لتمكين TLS 1.2، فأعيد تشغيل الخادم لكي يتم تفعيل التغييرات.</span><span class="sxs-lookup"><span data-stu-id="9c8e6-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="9c8e6-114">تأكد أيضا من تثبيت آخر تحديثات Windows و Exchange.</span><span class="sxs-lookup"><span data-stu-id="9c8e6-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="9c8e6-115">لمزيد من المعلومات، اطلع على:</span><span class="sxs-lookup"><span data-stu-id="9c8e6-115">For more information, see:</span></span>

- [<span data-ttu-id="9c8e6-116">إرشادات Exchange Server TLS، الجزء 1: الاستعداد ل TLS 1.2 - مجتمع Microsoft التقني</span><span class="sxs-lookup"><span data-stu-id="9c8e6-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="9c8e6-117">الجزء 2 من إرشادات Exchange Server TLS: تمكين TLS 1.2 وتحديد العملاء الذين لا يستخدمونه - مجتمع Microsoft التقني</span><span class="sxs-lookup"><span data-stu-id="9c8e6-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="9c8e6-118">فهم سيناريوهات البريد الإلكتروني إذا لم يتم الاتفاق على إصدارات TLS مع Exchange Online - مجتمع Microsoft التقني</span><span class="sxs-lookup"><span data-stu-id="9c8e6-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
