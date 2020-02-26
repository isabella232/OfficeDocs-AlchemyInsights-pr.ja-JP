---
title: Active Directory が同期しない
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "3754"
ms.openlocfilehash: 3abad160ab28922685d235a1fa546105e31757fb
ms.sourcegitcommit: d87a6ac6ee77375d1d750100359b4dc7b2871691
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/25/2020
ms.locfileid: "42268953"
---
# <a name="active-directory-not-syncing"></a>Active Directory が同期しない

"最近の同期がありません" のような同期エラーを受信している場合、または Office 管理ポータルのディレクトリ同期の状態が "前回の同期は3日前" であることが示されている場合は、AADConnect の設定が正しくないか、または不足している可能性があります。同期を実行するためのアクセス許可。  

エクスプレス設定を使用して AADConnect を再インストールすると、問題が迅速に解決する場合があります。

1. [AADConnect の最新バージョンをダウンロード](https://go.microsoft.com/fwlink/?LinkId=615771)します。

2. [高速インストールの手順に従い](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-install-express)ます。

AADConnect サービスアカウントの詳細については、「 [AZURE AD Connect: accounts and permissions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-accounts-permissions)」を参照してください。
