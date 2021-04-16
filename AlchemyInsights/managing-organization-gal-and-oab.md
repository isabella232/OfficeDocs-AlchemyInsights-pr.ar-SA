---
title: إدارة قائمة العناوين العمومية للمؤسسة ودفتر العناوين غير المتصل
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ar-SA
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794819"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="eaa6b-102">إدارة قائمة العناوين العمومية للمؤسسة ودفتر العناوين غير المتصل</span><span class="sxs-lookup"><span data-stu-id="eaa6b-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="eaa6b-103">قائمة العناوين العمومية هي قائمة من العناصر الممكَّنة للبريد (أي نوع من المستلمين يمكنه تلقي رسالة بريد إلكتروني) في المؤسسة.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="eaa6b-104">يتم تلقائياً إنشاء قائمة عناوين عمومية واحدة في كل مؤسسة.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="eaa6b-105">يمكنك إنشاء قائمة عناوين عمومية إضافية لفصل المستخدمين حسب المؤسسة أو الموقع، ولكن يمكن لمستخدم واحد فقط رؤية قائمة عناوين عمومية واحدة واستخدامها في المرة الواحدة.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="eaa6b-106">يمكنك لبعض تطبيقات "عميل البريد الإلكتروني"، مثل Outlook لنظام التشغيل Windows، تنزيل قائمة العناوين العمومية للاستخدام دون اتصال.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="eaa6b-107">يعرف ذلك بدفتر العناوين غير المتصل.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="eaa6b-108">يتم تحديث دفتر العناوين غير المتصل في Exchange online مرة واحدة فقط كل 8 ساعات، وبعد ذلك يجب على العملاء تنزيله لتحديث النسخة المحلية لدفتر العناوين غير المتصل الخاصة بهم.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="eaa6b-109">ويجب أن يكون أي تغيير في المستلمين مرئياً أولاً في قائمة العناوين العمومية لإجراءه لاحقاً في دفتر العناوين غير المتصل.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="eaa6b-110">فيما يلي بعض الإجراءات شائعة الاستخدام في قائمة العناوين العمومية ودفتر العناوين غير المتصل:</span><span class="sxs-lookup"><span data-stu-id="eaa6b-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="eaa6b-111">قد تحتاج لعدة أسباب إلى إخفاء بعض العناصر من قائمة العناوين العمومية.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="eaa6b-112">رجاءً راجع [إخفاء المستلمين من قوائم العناوين](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="eaa6b-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="eaa6b-113">إذا كنت بحاجة إلى منح مجموعات معينة من طرق العرض المخصصة للمستخدمين في قائمة العناوين العمومية لمؤسستك، فراجع [نُهج دفتر العناوين في Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="eaa6b-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="eaa6b-114">يمكنك [إنشاء قائمة عناوين عمومية في Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) وللتعرّف على طريقة العمل مع أذونات قائمة العناوين العمومية، راجع [قوائم العناوين في Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="eaa6b-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="eaa6b-115">رجاءً لاحظ أنك إذا أنشئت قوائم عناوين عمومية جديدة، فقد تحتاج أيضاً إلى إنشاء دفتر عناوين غير متصل جديد.</span><span class="sxs-lookup"><span data-stu-id="eaa6b-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="eaa6b-116">راجع [إجراءات دفتر العناوين غير المتصل](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="eaa6b-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
