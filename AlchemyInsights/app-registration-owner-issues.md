---
title: アプリ登録所有者の問題
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
- "9004352"
- "9655"
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951138"
---
# <a name="app-registration-owner-issues"></a>アプリ登録所有者の問題

以下は、アプリ登録の所有者としてプリンシパルを追加するために使用できる方法です。

- Azure AD PowerShell モジュールの使用 -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    参照: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI を使用する - `az ad app owner add`

    参照: [az 広告アプリの所有者](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph を使用する - 

    参照: [所有者を追加 - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Azure AD ポータルを使用する - [portal.azure.com](https://portal.azure.com/) > [AzureActiveDirectory] > [アプリの登録] > [アプリケーションの選択] > [所有者] > [所有者の追加] の順に移動します

**アプリケーションの所有者であるにもかかわらず、アプリ登録ブレードでアプリケーションを表示できませんか?**

アプリの所有者は管理者のロールとは異なります。 [[Azure AD 管理ポータルへのアクセスを制限する]](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) 設定が有効になっている場合、管理者だけがアプリ登録ポータルでアプリケーションを表示できます。 所有者がアプリケーションを表示できるようにするには、([いいえ]に設定して) この設定を無効にするか、特定のアプリケーションについてのみ所有者に管理者の役割を割り当てます。 ただし、このためには、Azure AD Premium P2 ライセンスがあること、および[特権 ID 管理](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)を有効にする必要があります。
