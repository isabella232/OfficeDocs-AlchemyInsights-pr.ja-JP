---
title: Active Directory が同期しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001688"
- "1300023"
- "3754"
- "4531"
ms.openlocfilehash: 0da512379e5a2f6ccb773e18c465e545c0660560
ms.sourcegitcommit: e42bb24c9bae1d0df8c49c424d2aa5e7466703ac
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2021
ms.locfileid: "52930980"
---
# <a name="active-directory-not-syncing"></a>Active Directory が同期しない

「同期が最近行われていません」などの同期エラーが表示される場合、または Office 管理ポータルでディレクトリ同期の状態が「最後の同期: 3 日以上前」と表示される場合は、AADConnect の設定が正しくないか、同期を実行するための権限が不十分である可能性があります。  

[簡単設定] を使用して AADConnect を再インストールすると、すぐに問題が解決する場合があります。

1. [AADConnect の最新バージョンをダウンロードします](https://go.microsoft.com/fwlink/?LinkId=615771)。

2. [高速インストール手順に従います](/azure/active-directory/hybrid/how-to-connect-install-express)。

Azure AD Connect は、Windows Server 2012 以降にインストールする必要があります。 このサーバーはドメイン参加型である必要があり、ドメイン コントローラーまたはメンバー サーバーの場合があります。 Azure AD Connect の要件と前提条件の完全なリストについては、[Azure AD Connect の前提条件](/azure/active-directory/hybrid/how-to-connect-install-prerequisites)をご覧ください。

AADConnect サービス アカウントの詳細については、「[Azure AD Connect: アカウントとアクセス許可](/azure/active-directory/hybrid/reference-connect-accounts-permissions)」を参照してください。
