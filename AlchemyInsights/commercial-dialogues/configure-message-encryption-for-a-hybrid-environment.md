---
title: تكوين تشفير الرسائل لبيئة مختلطة
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 03/11/2021
ms.locfileid: "50742997"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a><span data-ttu-id="0ab04-102">تكوين تشفير الرسائل لبيئة مختلطة</span><span class="sxs-lookup"><span data-stu-id="0ab04-102">Configure message encryption for a hybrid environment</span></span>

<span data-ttu-id="0ab04-103">بالنسبة لبيئات Exchange المختلطة، يمكن للمستخدمين المحليين إرسال بريد إلكتروني مشفر باستخدام تشفير رسائل Office (OME) فقط إذا تم توجيه البريد الإلكتروني عبر Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="0ab04-103">For hybrid Exchange environments, on-premises users can send encrypted email using Office Message Encryption (OME) only if email is routed through Exchange Online.</span></span>

<span data-ttu-id="0ab04-104">لتشفير رسائل البريد الإلكتروني باستخدام OME، تنفيذ الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="0ab04-104">To encrypt emails using OME, perform the following steps:</span></span>

1. <span data-ttu-id="0ab04-105">استخدم معالج [التكوين المختلط](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) لإعداد البيئة المختلطة.</span><span class="sxs-lookup"><span data-stu-id="0ab04-105">Use the [Hybrid Configuration wizard](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard) to set up your hybrid environment.</span></span> <span data-ttu-id="0ab04-106">لا يلزم اتخاذ خطوات خاصة لإعداد التشفير.</span><span class="sxs-lookup"><span data-stu-id="0ab04-106">No special steps are required for setting up encryption.</span></span>
2. <span data-ttu-id="0ab04-107">[قم بإعداد قواعد تدفق البريد للتشفير](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) كما لو كنت تقوم بذلك عادة.</span><span class="sxs-lookup"><span data-stu-id="0ab04-107">[Set up your mail flow rules for encryption](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email) like you normally would.</span></span>


