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
# <a name="sharepoint-online-powershell"></a>SharePoint Online の PowerShell

Sharepoint Online 内で PowerShell またはスクリプトを使用していますか ? 詳細については、以下のリンクをご覧ください。
- [SharePoint Online 管理シェルの使用を開始する](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [多要素認証 (MFA) を使用して SPO PowerShell に接続する場合](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint のパターンとプラクティス (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) には、SPO に対する複雑な管理アクションを実行できる PowerShell コマンドのライブラリが含まれています。

> [!NOTE]
> - SPO 管理シェルとの接続に問題がある場合には、最新バージョンに更新したことを確認し、[モジュールの再インポート](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)を試します。その際、*“Import-Module Microsoft.Online.SharePoint.PowerShell”* を使用してください。
> - クライアント側のオブジェクト モデル スクリプトを実行しようとする場合、ローカル マシンに [Sharepoint Online クライアント コンポーネント SDK](https://www.microsoft.com/download/details.aspx?id=42038) をインストールする必要があります。
> - PowerShell からのスクリプトの実行に問題がある場合には、管理者として PowerShell を実行し、[実行ポリシー](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)の変更を検討してください。