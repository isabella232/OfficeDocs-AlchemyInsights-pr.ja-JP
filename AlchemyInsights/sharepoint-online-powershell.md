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
# <a name="sharepoint-online-powershell"></a>Sharepoint Online PowerShell

Sharepoint Online 内の PowerShell またはスクリプトを使用する場合 詳細については、以下のリンク先を参照してください。
- [SharePoint Online 管理シェルの概要](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [多要素認証 (MFA) を使用して SPO PowerShell に接続する](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- [SharePoint のパターンとプラクティス (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps)には、spo に対して複雑な管理操作を実行できる PowerShell コマンドのライブラリが含まれています。

> [!NOTE]
> - SPO 管理シェルとの接続で問題が発生している場合は、最新バージョンに更新されていることを確認してから、 *"import-Module Microsoft. PowerShell"* を使用して[モジュールを再インポート](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module)してください。
> - クライアント側オブジェクトモデルスクリプトを実行しようとしている場合は、 [Sharepoint Online クライアントコンポーネント SDK](https://www.microsoft.com/download/details.aspx?id=42038)をローカルコンピューターにインストールする必要があります。
> - PowerShell からスクリプトを実行するときに問題が発生した場合は、PowerShell を管理者として実行し、[実行ポリシー](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6)を変更することを検討してください。