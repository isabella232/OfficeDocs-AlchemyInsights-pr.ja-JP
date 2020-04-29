---
title: SharePoint Online の PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 8c270748fc75f929371fbb2856daad3ae61a1540
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764266"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fc812-102">SharePoint Online の PowerShell</span><span class="sxs-lookup"><span data-stu-id="fc812-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fc812-103">Sharepoint Online 内で PowerShell またはスクリプトを使用していますか ?</span><span class="sxs-lookup"><span data-stu-id="fc812-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fc812-104">詳細については、以下のリンクをご覧ください。</span><span class="sxs-lookup"><span data-stu-id="fc812-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fc812-105">SharePoint Online 管理シェルの使用を開始する</span><span class="sxs-lookup"><span data-stu-id="fc812-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fc812-106">多要素認証 (MFA) を使用して SPO PowerShell に接続する場合</span><span class="sxs-lookup"><span data-stu-id="fc812-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fc812-107">[SharePoint のパターンとプラクティス (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) には、SPO に対する複雑な管理アクションを実行できる PowerShell コマンドのライブラリが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fc812-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fc812-108">SPO 管理シェルとの接続に問題がある場合には、最新バージョンに更新したことを確認し、[モジュールの再インポート](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)を試します。その際、*“Import-Module Microsoft.Online.SharePoint.PowerShell”* を使用してください。</span><span class="sxs-lookup"><span data-stu-id="fc812-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fc812-109">クライアント側のオブジェクト モデル スクリプトを実行しようとする場合、ローカル マシンに [Sharepoint Online クライアント コンポーネント SDK](https://www.microsoft.com/download/details.aspx?id=42038) をインストールする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc812-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fc812-110">PowerShell からのスクリプトの実行に問題がある場合には、管理者として PowerShell を実行し、[実行ポリシー](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)の変更を検討してください。</span><span class="sxs-lookup"><span data-stu-id="fc812-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>