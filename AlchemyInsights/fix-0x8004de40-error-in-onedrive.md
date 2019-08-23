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
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525064"
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