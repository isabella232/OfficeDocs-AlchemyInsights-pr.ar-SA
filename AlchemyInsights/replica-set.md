---
title: مجموعة النسخ المتماثلة
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/10/2021
ms.locfileid: "50713306"
---
# <a name="replica-set"></a><span data-ttu-id="6bec6-102">مجموعة النسخ المتماثلة</span><span class="sxs-lookup"><span data-stu-id="6bec6-102">Replica set</span></span>

<span data-ttu-id="6bec6-103">ويسمى أيضا AADDS كمجال مدار.</span><span class="sxs-lookup"><span data-stu-id="6bec6-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="6bec6-104">في الواقع، يوجد اثنين من وحدات تحكم المجالات التي يتم تشغيلها وصيانتها بواسطة الواجهة الخلفية.</span><span class="sxs-lookup"><span data-stu-id="6bec6-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="6bec6-105">يتضمن كل من المكاتين DC رئيسي واحد و DC متماثلا واحدا.</span><span class="sxs-lookup"><span data-stu-id="6bec6-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="6bec6-106">النسخ الاحتياطية في AADDS (المجال المدار) هي عملية تلقائية مدارة بواسطة نظام Azure الأساسي.</span><span class="sxs-lookup"><span data-stu-id="6bec6-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="6bec6-107">في حالة وجود مشكلة في مجالك المدار، يمكن أن يساعدك دعم Azure في الاستعادة من النسخ الاحتياطي.</span><span class="sxs-lookup"><span data-stu-id="6bec6-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="6bec6-108">يمكنك إنشاء كل نسخة مماثلة تم تعيينها في شبكة ظاهرية.</span><span class="sxs-lookup"><span data-stu-id="6bec6-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="6bec6-109">يجب أن يتم أقران كل شبكة ظاهرية إلى كل شبكة ظاهرية أخرى تستضيف مجموعة النسخ المتماثلة لمجال مدار.</span><span class="sxs-lookup"><span data-stu-id="6bec6-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="6bec6-110">ينشئ هذا التكوين شبكة شبكة طبولوجيا تدعم تكرار الدليل.</span><span class="sxs-lookup"><span data-stu-id="6bec6-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="6bec6-111">يمكن للشبكة الظاهرية دعم مجموعات نسخ مماثلة متعددة، شرط أن تكون كل مجموعة نسخ مماثلة في شبكة فرعية ظاهرية مختلفة.</span><span class="sxs-lookup"><span data-stu-id="6bec6-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="6bec6-112">لمزيد من التفاصيل حول مجموعة النسخ المتماثلة، راجع [مجموعات النسخ المتماثلة ل "المفاهيم".](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)</span><span class="sxs-lookup"><span data-stu-id="6bec6-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
