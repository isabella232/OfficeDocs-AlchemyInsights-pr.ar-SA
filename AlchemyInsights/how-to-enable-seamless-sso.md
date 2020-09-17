---
title: كيفيه تمكين SSO السلس
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "628"
- "1300012"
ms.assetid: 80c88b2d-adb1-4e45-8eff-aaa80403b5b6
ms.openlocfilehash: f3581549823e1ec650a3717780bc07e9944d4c1c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ar-SA
ms.lasthandoff: 09/15/2020
ms.locfileid: "47780514"
---
# <a name="how-to-enable-seamless-sso"></a><span data-ttu-id="d4a48-102">كيفيه تمكين SSO السلس</span><span class="sxs-lookup"><span data-stu-id="d4a48-102">How to enable Seamless SSO</span></span>

<span data-ttu-id="d4a48-103">تمكين SSO السلس عبر [AZURE AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span><span class="sxs-lookup"><span data-stu-id="d4a48-103">Enable Seamless SSO through [Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect).</span></span>
  
<span data-ttu-id="d4a48-104">إذا كنت تقوم بتثبيت حديث ل Azure AD Connect ، فاختر [مسار التثبيت المخصص](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span><span class="sxs-lookup"><span data-stu-id="d4a48-104">If you're doing a fresh installation of Azure AD Connect, choose the [custom installation path](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-get-started-custom).</span></span> <span data-ttu-id="d4a48-105">في صفحه **تسجيل الدخول إلى المستخدم** ، حدد الخيار **تمكين تسجيل الدخول الأحادي** .</span><span class="sxs-lookup"><span data-stu-id="d4a48-105">At the **User sign-in** page, choose the **Enable single sign-on** option.</span></span>
  
<span data-ttu-id="d4a48-106">للتحقق من انك قمت بتمكين SSO السلسة بشكل صحيح:</span><span class="sxs-lookup"><span data-stu-id="d4a48-106">To verify that you have enabled Seamless SSO correctly:</span></span>
  
1. <span data-ttu-id="d4a48-107">سجل دخولك إلى [مركز أداره Azure active](https://aad.portal.azure.com) directory كمسؤول عام.</span><span class="sxs-lookup"><span data-stu-id="d4a48-107">Sign in to the [Azure Active Directory administrative center](https://aad.portal.azure.com) as a global admin.</span></span>

2. <span data-ttu-id="d4a48-108">حدد **Azure active** directory في الجزء الأيمن.</span><span class="sxs-lookup"><span data-stu-id="d4a48-108">Select **Azure Active Directory** in the left pane.</span></span>

3. <span data-ttu-id="d4a48-109">تاكد من **تمكين**تسجيل الدخول الأحادي السلس.</span><span class="sxs-lookup"><span data-stu-id="d4a48-109">Verify that Seamless single sign-on is **Enabled**.</span></span>

<span data-ttu-id="d4a48-110">لمعرفه المزيد ، راجع [تسجيل الدخول الأحادي السلس في Azure Active directory: البدء السريع](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span><span class="sxs-lookup"><span data-stu-id="d4a48-110">To learn more, see [Azure Active Directory Seamless Single Sign-On: Quick start](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-sso-quick-start).</span></span>
  