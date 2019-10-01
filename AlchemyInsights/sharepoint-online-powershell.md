---
title: Sharepoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2019
ms.locfileid: "37313931"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6d187-102">Sharepoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="6d187-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6d187-103">Sharepoint Online 内の PowerShell またはスクリプトを使用する場合</span><span class="sxs-lookup"><span data-stu-id="6d187-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6d187-104">詳細については、以下のリンク先を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6d187-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6d187-105">SharePoint Online 管理シェルの概要</span><span class="sxs-lookup"><span data-stu-id="6d187-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6d187-106">多要素認証 (MFA) を使用して SPO PowerShell に接続する</span><span class="sxs-lookup"><span data-stu-id="6d187-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6d187-107">[SharePoint のパターンとプラクティス (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)には、spo に対して複雑な管理操作を実行できる PowerShell コマンドのライブラリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6d187-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6d187-108">SPO 管理シェルとの接続で問題が発生している場合は、最新バージョンに更新されていることを確認してから、 *"import-Module Microsoft. PowerShell"* を使用して[モジュールを再インポート](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)してください。</span><span class="sxs-lookup"><span data-stu-id="6d187-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6d187-109">クライアント側オブジェクトモデルスクリプトを実行しようとしている場合は、 [Sharepoint Online クライアントコンポーネント SDK](https://www.microsoft.com/download/details.aspx?id=42038)をローカルコンピューターにインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d187-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6d187-110">PowerShell からスクリプトを実行するときに問題が発生した場合は、PowerShell を管理者として実行し、[実行ポリシー](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)を変更することを検討してください。</span><span class="sxs-lookup"><span data-stu-id="6d187-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>