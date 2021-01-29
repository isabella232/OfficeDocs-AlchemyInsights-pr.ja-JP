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
# <a name="delete-or-restore-applications"></a>アプリケーションの削除または復元

**Azure AD テナントからアプリケーションを削除するには**:

1. **Azure AD ポータル** で、**[エンタープライズ アプリケーション]** を選択します。 次に、削除するアプリケーションを見つけて選択します。
2. 左側のペインの **[管理]** セクションで、**[プロパティ]** を選択します。
3. **[削除]** を選択し、**[はい]** を選択して、Azure AD テナントからアプリを削除することを確認します。

アプリを削除する方法の詳細については、「[クイックスタート: Azure Active Directory (Azure AD) テナントからアプリケーションを削除する](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)」を参照してください。

PowerShellでは、[Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) コマンドレットを使って、Azure Active Directory 内の特定のアプリケーションからアプリケーションプロキシ構成を削除し、指定されている場合はアプリケーションを完全に削除できます。

PowerShell を使用して、**削除したアプリケーションを復元** できます。 復元するアプリケーションが特定されたら、[Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication) を使用して復元できます。
