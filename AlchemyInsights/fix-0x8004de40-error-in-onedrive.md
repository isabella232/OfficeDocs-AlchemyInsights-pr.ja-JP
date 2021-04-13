---
title: OneDrive のエラー 0x8004de40 の修正
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649753"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive のエラー 0x8004de40 の修正

Windows 7 を実行していてこのエラーが発生した場合は、[更新して、Windows の WinHTTP で TLS 1.1 および TLS 1.2 を既定の安全なプロトコルとして有効にします](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

Windows 10 を実行していて、OneDrive で 0x8004de40 エラーが発生した場合:

- Acitve ディレクトリ ドメインに接続されている間に、影響を受けたコンピューターを再起動します。
- 再起動で問題が修正しない場合は、Azure AD からデバイスを切断してから再度参加させます。 

**注**: 次の手順を実行している間、社内ネットワーク上にいなければなりません。 例えば旅行中など、社内インフラストラクチャに接続できない場合は、これらの手順を実行しないでください。 

1. **[スタート]** を選択し、**[コマンド プロンプト]** を右クリックして **[管理者として実行]** を選択し、管理者特権でのコマンド プロンプトを開きます。

1. 「*dsregcmd /leave*」と入力して **Enter** キーを押します。

1. 操作が終了したら、「*dsregcmd /join*」と入力して **Enter** キーを押します。

1. 完了したら、コマンド プロンプトを閉じます。

1. コンピューターを再起動して、OneDrive にログインします。