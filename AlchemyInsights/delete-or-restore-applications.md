---
title: アプリケーションの削除または復元
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
- "9004335"
- "7737"
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/27/2021
ms.locfileid: "50015072"
---
# <a name="delete-or-restore-applications"></a><span data-ttu-id="835c3-102">アプリケーションの削除または復元</span><span class="sxs-lookup"><span data-stu-id="835c3-102">Delete or restore applications</span></span>

<span data-ttu-id="835c3-103">**Azure AD テナントからアプリケーションを削除するには**:</span><span class="sxs-lookup"><span data-stu-id="835c3-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="835c3-104">**Azure AD ポータル** で、**[エンタープライズ アプリケーション]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="835c3-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="835c3-105">次に、削除するアプリケーションを見つけて選択します。</span><span class="sxs-lookup"><span data-stu-id="835c3-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="835c3-106">左側のペインの **[管理]** セクションで、**[プロパティ]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="835c3-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="835c3-107">**[削除]** を選択し、**[はい]** を選択して、Azure AD テナントからアプリを削除することを確認します。</span><span class="sxs-lookup"><span data-stu-id="835c3-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="835c3-108">アプリを削除する方法の詳細については、「[クイックスタート: Azure Active Directory (Azure AD) テナントからアプリケーションを削除する](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="835c3-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="835c3-109">PowerShellでは、[Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) コマンドレットを使って、Azure Active Directory 内の特定のアプリケーションからアプリケーションプロキシ構成を削除し、指定されている場合はアプリケーションを完全に削除できます。</span><span class="sxs-lookup"><span data-stu-id="835c3-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="835c3-110">PowerShell を使用して、**削除したアプリケーションを復元** できます。</span><span class="sxs-lookup"><span data-stu-id="835c3-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="835c3-111">復元するアプリケーションが特定されたら、[Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) を使用して復元できます。</span><span class="sxs-lookup"><span data-stu-id="835c3-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
