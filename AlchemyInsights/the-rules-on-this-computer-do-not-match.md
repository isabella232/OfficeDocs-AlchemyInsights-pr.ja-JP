---
title: 'エラー: このコンピューターのルールは一致しません'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: b77573e9d94195e1f0ef4a1566c45a30d53b7e68e502aeb834e2ca5b9e6c5c76
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53981118"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a>エラー: このコンピューターのルールは一致しません

この既知の問題の最新の状態を確認するには、「[このコンピューターのルールが Microsoft Exchange のルールと一致しない](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)」を参照してください。

Outlook チームは、ビルド 12928.10000 で修正プログラムを実装しました。 この修正プログラムは既に Insider ファーストで利用できます。また、2020 年 6 月後半には、月次チャネルでも利用可能になります。 修正プログラムのビルドが完了すると、「保持したいルールを選んでください」というメッセージが表示される場合があります。 メッセージが表示されたら、[サーバー] を選んでから、Outlook に戻り、無効になっていたルールを再び有効にします。

修正プログラムが使用可能になるまで、次の回避策を使用してください。

**回避策**: 最新のレポートでは、Outlook デスクトップでクライアント ルールを作成しただけのユーザーにこの問題が発生しています。 問題の発生が続く場合は、該当のルールを削除してから、OWA (Outlook Web App) で、問題が解消するまでルールを作成、編集します。

ルールを手動で削除できない場合は、Outlook を起動する時にOutlook.exe /cleanrules を実行することで Outlook のコマンドを実行できます。 これにより、クライアントとサーバー両方のルールが削除されます。 Outlook プロファイル内すべてのアカウントの全ルールが削除されます。 このコマンドについては詳しくは、コマンド ライン スイッチの記事に記載されています。

