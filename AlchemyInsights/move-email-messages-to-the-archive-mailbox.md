---
title: نقل رسائل البريد الإلكتروني إلى أرشيف علبة البريد
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 41d6825b568263fb7b09066b65235aa348415bae
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 01/24/2019
ms.locfileid: "29455941"
---
<span data-ttu-id="3a45f-p101">مشاكل أرشفة العناصر إلى أرشيف علبة البريد. تأكد من قيامك بتنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="3a45f-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="3a45f-p102">تأكد من أن **أرشفة علبة البريد** تم تمكينه. إذا لم يكن الأمر كذلك، استخدم الخطوات في [هذه المقالة](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) لتمكين علبة البريد الأرشيف.</span><span class="sxs-lookup"><span data-stu-id="3a45f-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/en-us/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="3a45f-106">في مركز مسؤول Exchange، حدد **علامات الاستبقاء** تحت **إدارة التوافق**، إنشاء **علامة استبقاء** مع عمل **نقل أرشيف** يتضمن المطلوب **الاستبقاء**.</span><span class="sxs-lookup"><span data-stu-id="3a45f-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="3a45f-107">في مركز مسؤول Exchange، حدد **نهج الاستبقاء**وإنشاء **نهج الاستبقاء** وإضافة علامة استبقاء **نقل أرشيف** لذلك النهج.</span><span class="sxs-lookup"><span data-stu-id="3a45f-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="3a45f-p103">[تعيين "نهج الاستبقاء"](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) لعلبة البريد لمستخدم معين. سيتم تطبيق نفس النهج **الأساسي** و **أرشيف** علبة البريد.</span><span class="sxs-lookup"><span data-stu-id="3a45f-p103">[Assign the Retention Policy](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="3a45f-p104">علبة بريد المستخدم يجب الآن نهج أرشيف لنقل العناصر إلى أرشيف علبة البريد. قد يكون من الضروري فرض إدارة مجلد مساعد (وزارة الخارجية) لتشغيل وتطبيق الإعدادات الجديدة بعلبة بريد مستخدم. تشغيل الأمر التالي أثناء [الاتصال ب PowerShell أكسو](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) لبدء إدارة "مساعد المجلدات" لعلبة بريد محددة:</span><span class="sxs-lookup"><span data-stu-id="3a45f-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="3a45f-113">للمزيد من المعلومات حول إعداد نهج أرشيف، راجع [إعداد نهج الأرشيف والحذف لعلب البريد](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span><span class="sxs-lookup"><span data-stu-id="3a45f-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/en-us/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

