---
title: OneDrive での0x8004de40 エラーの修正
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2019
ms.locfileid: "35174671"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive での0x8004de40 エラーの修正

OneDrive を使用してエラーを受信した場合は、次のようにします。

- Acitve Directory ドメインに接続している間に、影響を受けたコンピューターを再起動します。
- 再起動しても問題が解決されない場合は、Azure AD からデバイスを分離して再参加させてください。 

**注**: これらの手順を実行している間は、企業ネットワークにログオンする必要があります。 企業インフラストラクチャ (出張中など) に接続できない場合は、これらの手順を実行しないでください。 

- 管理者特権でのコマンド プロンプトを開きます。 
- 昇格したコマンドプロンプトを開くには、[**スタート**] をクリックし、[**コマンドプロンプト**] を右クリックし、[**管理者として実行**] をクリックします。
- 「 *Dsregcmd/Leave* 」と入力し、 **enter**キーを押します。
- 完了したら、「 *dsregcmd/join* 」と入力し、 **enter**キーを押します。
- 完了したら、コマンドプロンプトを閉じます。
- コンピューターを再起動して、OneDrive にログインします。