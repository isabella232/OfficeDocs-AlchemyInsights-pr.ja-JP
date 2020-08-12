---
title: Mac 用の Teams アドイン
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/10/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6173"
- "9003233"
ms.openlocfilehash: 74bd424f71a59b80a91b960b815363668bee7036
ms.sourcegitcommit: 1361b2b37fd0201502a1a3547084961de284a3fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2020
ms.locfileid: "46630079"
---
# <a name="teams-add-in-for-mac"></a>Mac 用の Teams アドイン

Mac オペレーティング システム ユーザー用の Teams アドインが存在しない問題のトラブルシューティングを行うには、次の手順を実行します。

**手順 1:** Hybrid Exchange オンプレミス（2016 CU3 以降に必要）を所有している場合は、 Test-HMA.ps1 ツールを使用してハイブリッド先進認証が正しく構成されていることを確認します。 詳細については、[「iOS および Android 用の Outlook でのハイブリッド先進認証の検証」](https://aka.ms/AA980zq) を参照してください。  

**注:** domain\username ではなく、UPN のアドレス形式（たとえば、[username@contoso.com](mailto:username@contoso.com)）を使用してください。 Exchange Online メールボックスを使用するユーザーの場合でも、この操作を行います。

**手順 2:** **ツール** > **アカウント**に移動します。Mac 用 Outlook で、アカウントを見つけて選択します。 表示されているユーザー名が[username@contoso.com](mailto:username@contoso.com) のような UPN 形式であることを確認します。

**手順 3:** ユーザーがライセンス認証を受けた Microsoft Teams ユーザーであることを確認します。 ユーザーは、Mac 用 Office 365 サブスクリプションの製品バージョン 16.24 以降を使用している必要があります。