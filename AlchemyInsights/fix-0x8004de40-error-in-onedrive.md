---
title: OneDrive のエラー 0x8004de40 の修正
ms.author: pebaum
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: aa0e0a63ac1e365a7cdce018626740446040a664
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/04/2019
ms.locfileid: "36755853"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>OneDrive のエラー 0x8004de40 の修正

OneDrive でエラー 0x8004de40 が発生した場合は、次の操作を実行します。

- Acitve ディレクトリ ドメインに接続されている間に、影響を受けたコンピューターを再起動します。
- 再起動で問題が修正しない場合は、Azure AD からデバイスを切断してから再度参加させます。 

**注**: 次の手順を実行している間、社内ネットワーク上にいなければなりません。 例えば旅行中など、社内インフラストラクチャに接続できない場合は、これらの手順を実行しないでください。 

- 管理者特権でコマンド プロンプトを開きます。 
- 管理者特権でコマンド プロンプトを開くには、[**スタート**] をクリックし、[**コマンド プロンプト**] を右クリックして、[**管理者として実行**] をクリックします。
- 「*dsregcmd /leave*」と入力して**Enter**キーを押します。
- 操作が終了したら、「*dsregcmd /join*」と入力して**Enter**キーを押します。
- 完了したら、コマンド プロンプトを閉じます。
- コンピューターを再起動して、OneDrive にログインします。