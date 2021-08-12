---
title: 組織内の電子メールメッセージの検索と削除
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: bd25d9bb2af8114786503e129de105c9a0f602c98b206f01770605d1957e3a1b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53948888"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a>組織内の電子メールメッセージの検索と削除

次の手順を実行します。

1. グローバル管理者ではない場合、メッセージを検索するには、自分のアカウントを **電子情報開示マネージャー役割グループ** または **コンプライアンス検索管理の役割** に追加する必要があります。 メッセージを削除するには、**組織管理の役割グループ** のメンバーであるか、**検索と消去の管理の役割** が割り当てられている必要があります。 これらの役割へのアクセス許可は、[セキュリティ/コンプライアンス センター](https://protection.office.com)で割り当てられます。
2. [コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。
3. [セキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。 MFA をお使いの場合は、「[多要素認証を使用してセキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)」の手順を参照してください。
4. メッセージを削除します。`New-ComplianceSearchAction` コマンドレットを実行してメッセージを削除します。 削除されたメッセージは、ユーザーの [回復可能なアイテム] フォルダーに移動します。 コマンドの例については、「[手順 3: メッセージを削除する](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)」を参照してください。
