---
title: تعيين الإصدارات في SharePoint و OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: a84868ba-7657-4f34-8a57-df9c6f9732dc
ms.custom:
- "5300025"
- "1702"
ms.openlocfilehash: 12207efc9822be6cf096fa4884a3cd244a286cbe
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47800811"
---
# <a name="versioning-in-sharepoint-and-onedrive"></a><span data-ttu-id="d3d7b-102">تعيين الإصدارات في SharePoint و OneDrive</span><span class="sxs-lookup"><span data-stu-id="d3d7b-102">Versioning in SharePoint and OneDrive</span></span> 


<span data-ttu-id="d3d7b-103">عند تمكين تعيين الإصدار في قائمه أو مكتبه SharePoint ، يمكنك تخزين العناصر وتعقبها واستعادتها في قائمه وملفات في مكتبه عند تغييرها.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-103">When versioning is enabled in your SharePoint list or library, you can store, track, and restore items in a list and files in a library whenever they change.</span></span> <span data-ttu-id="d3d7b-104">يوفر لك تعيين الإصدارات التي يتم دمجها مع الإعدادات الأخرى ، مثل السحب ، الكثير من التحكم في المحتوي الذي يتم نشره علي موقعك ويمكنه توفير قيمه حقيقية إذا كنت بحاجه إلى إلقاء نظره علي الإصدار القديم من عنصر أو ملف أو استعادته.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-104">Versioning, combined with other settings, such as checkout, gives you a lot of control of the content that is posted on your site and can provide real value if you ever have a need to look at or restore an old version of an item or file.</span></span>

<span data-ttu-id="d3d7b-105">للحصول علي مزيد من المعلومات حول تعيين الإصدار يرجى زيارة المقالات التالية.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-105">For more information on versioning please visit the below articles.</span></span>

- [<span data-ttu-id="d3d7b-106">كيف تعمل ميزه تعيين الإصدار في قائمه أو مكتبه SharePoint</span><span class="sxs-lookup"><span data-stu-id="d3d7b-106">How does versioning work in a SharePoint list or library</span></span>](https://support.office.com/article/how-does-versioning-work-in-a-sharepoint-list-or-library-0f6cd105-974f-44a4-aadb-43ac5bdfd247)

- [<span data-ttu-id="d3d7b-107">تمكين تعيين الإصدار لقائمه أو مكتبه وتكوينه</span><span class="sxs-lookup"><span data-stu-id="d3d7b-107">Enable and configure versioning for a list or library</span></span>](https://support.office.com/article/enable-and-configure-versioning-for-a-list-or-library-1555d642-23ee-446a-990a-bcab618c7a37?ocmsassetID=HA102772148&amp;CTT=3&amp;CorrelationId=52441bb1-a619-4375-89d5-19d28769890f)

- [<span data-ttu-id="d3d7b-108">كيفيه عرض محفوظات الإصدارات</span><span class="sxs-lookup"><span data-stu-id="d3d7b-108">How to view version history</span></span>](https://support.office.com/article/View-the-version-history-of-an-item-or-file-in-a-list-or-library-53262060-5092-424D-A50B-C798B0EC32B1)

- [<span data-ttu-id="d3d7b-109">استعاده إصدار سابق من ملف في OneDrive</span><span class="sxs-lookup"><span data-stu-id="d3d7b-109">Restore a previous version of a file in OneDrive</span></span>](https://support.office.com/article/restore-a-previous-version-of-a-file-in-onedrive-159cad6d-d76e-4981-88ef-de6e96c93893)

- [<span data-ttu-id="d3d7b-110">عرض الإصدارات السابقة من ملفات Office</span><span class="sxs-lookup"><span data-stu-id="d3d7b-110">View previous versions of Office files</span></span>](https://support.office.com/article/view-previous-versions-of-office-files-5c1e076f-a9c9-41b8-8ace-f77b9642e2c2)

- [<span data-ttu-id="d3d7b-111">حدود تعيين الإصدارات</span><span class="sxs-lookup"><span data-stu-id="d3d7b-111">Versioning limits</span></span>](https://docs.microsoft.com/office365/servicedescriptions/sharepoint-online-service-description/sharepoint-online-limits)

>[!Note] 
><span data-ttu-id="d3d7b-112">إذا كنت عميل Microsoft 365 ، سيتم الآن تشغيل تعيين الإصدار بشكل افتراضي عند إنشاء مكتبات OneDrive for business جديده ، سيتم تلقائيا حفظ الإصدارات ال500 أخيره من المستند.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-112">If you are a Microsoft 365 customer, versioning is now turned on by default when you create new OneDrive for Business libraries, and it will automatically save the last 500 versions of a document.</span></span> <span data-ttu-id="d3d7b-113">سيساعدك هذا في منع فقدان المستندات أو البيانات المهمة.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-113">This will help you prevent losing important documents or data.</span></span> <span data-ttu-id="d3d7b-114">إذا كانت لديك مكتبات موجودة علي موقع OneDrive for Business أو علي موقع الفريق الذي لم يتم تمكين تعيين الإصدار له ، فيمكنك تشغيل ميزه تعيين الإصدار في اي وقت.</span><span class="sxs-lookup"><span data-stu-id="d3d7b-114">If you have existing libraries on your OneDrive for Business site or on your team site that do not have versioning enabled, you can turn versioning on for them at any time.</span></span>


