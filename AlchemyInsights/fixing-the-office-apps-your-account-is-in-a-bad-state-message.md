---
title: إصلاح تطبيقات Office حسابك في رسالة حالة سيئة
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969187"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="8b6d1-102">إصلاح تطبيقات Office "حسابك في حالة سيئة" خطأ</span><span class="sxs-lookup"><span data-stu-id="8b6d1-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="8b6d1-103">لإصلاح هذا الخطأ، حاول الخيارات التالية على الكمبيوتر المتأثر:</span><span class="sxs-lookup"><span data-stu-id="8b6d1-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="8b6d1-104">فتح تطبيق Office، حدد تسجيل خروج**حساب** >  **الملف** > **من جميع الحسابات**.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="8b6d1-105">تسجيل الدخول مرة أخرى باستخدام حساب مستخدم بترخيص صالح.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="8b6d1-106">للحصول على معلومات تفصيلية، راجع [الحسابات في Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="8b6d1-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="8b6d1-107">[مسح بيانات اعتماد Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) باستخدام إدارة بيانات اعتماد Windows.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="8b6d1-108">**ملاحظة:** تغيرت مسارات التسجيل لـ Office 2016 إلى 16.0.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="8b6d1-109">على سبيل المثال، \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="8b6d1-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="8b6d1-110">على الكمبيوتر المتأثر، قم بتعيين EnableADAL = 0 باستخدام الخطوات التالية:</span><span class="sxs-lookup"><span data-stu-id="8b6d1-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="8b6d1-111">انقر بزر Windows وحدد **تشغيل**.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="8b6d1-112">في المربع **المفتوح،** اكتب **regedit**، ثم حدد **موافق**.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="8b6d1-113">حدد **نعم** عند المطالبة للسماح لمحرر التسجيل بإجراء تغييرات على جهازك.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="8b6d1-114">في محرر التسجيل، قم بإضافة قيمة DWORD من EnableADAL مع إعداد 0 تحت HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="8b6d1-115">إذا حدث الخطأ أثناء الاتصال بـ Office 365 باستخدام Office 2013، [قم بتمكين المصادقة الحديثة](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) لعميل Office.</span><span class="sxs-lookup"><span data-stu-id="8b6d1-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="8b6d1-116">لمزيد من المعلومات، راجع [كيفية استكشاف الأخطاء وإصلاحها للتطبيقات غير المستعرض التي لا يمكنها تسجيل الدخول إلى Office 365 أو Azure أو Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="8b6d1-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

