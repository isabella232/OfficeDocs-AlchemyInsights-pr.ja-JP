---
title: Teams のプライベート チャネルを削除する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440563"
---
# <a name="delete-a-teams-private-channel"></a>Teams のプライベート チャネルを削除する

Microsoft は、もし基になる SharePoint サイトに対して SharePoint アイテム保持ポリシーが有効だと、Teams のプライベート チャネルが削除されるという問題を認識しています。 Microsoft は解決に取り組んでいます。 それまでは、次の回避策を使用してプライベート チャネルを削除できます。

**Sharepoint アイテム保持ポリシーから Team /サイトコレクションを除外します。**

1. Office 365 管理ポータルに移動し、左側のナビゲーション ウィンドウで [**すべて表示**] を選択します。
2. [**管理センター**] の下にある [**セキュリティ/コンプライアンス** > **データ損失防止** > **ポリシー**] に移動します。
3. Sharepoint サイトに適用されるポリシーすべてを特定し、プライベート チャネルを含む Team の Sharepoint サイトがアイテム保持ポリシーに含まれないように、そのポリシーを変更します。
4. ポリシーを保存します。
    ポリシー設定が有効になるまで最大 24 時間かかる場合があります。
    サイトを除外したら、プライベート チャネルを削除できます。  
    
お客様の Android デバイスで Microsoft Teams を使用すると、プライベート チャネルを削除できる ***可能性*** があります。 

関連する SharePoint の詳細については、[SharePoint Online または OneDrive for Business でアイテムを削除できない](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)を参照してください。