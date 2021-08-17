---
title: 既存のブラウザー環境を評価し、目標を定義する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: ff965b3f2fd747763185fcf4cd43479b1cd7189ed737005c2aca4a723df135cb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54043661"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a>既存のブラウザー環境を評価し、目標を定義する

時間をかけて現在のブラウザーの状態とプロジェクトのビジョンを理解することで、すべてのプロジェクト関係者が一致して、同じ目標に向けて取り組むことができます。次の手順に従ってください。

1. 現在の状態を定義する。 次の状況について検討しましょう。
- 現在、どのブラウザーが環境に展開されていますか?
- どのブラウザーが既定のブラウザーとして設定されていますか?
- 一部のアプリで Internet Explorer を使用する必要がありますか?
- エンタープライズ モード のサイト リストを使用して、現在使っている Internet Explorer を構成していますか?
- お使いの環境でサポートされている OS プラットフォーム(Windows 10やmacOSなど)はどれですか？ 
- ブラウザー管理には、どの管理ツールを使用しますか?
- ブラウザーの構成と管理の責任者
- ブラウザーの互換性を検証するためのプロセス
2. 展開の目標を定義する。 以下の点に注意してください。
- [Microsoft Edge を既定のブラウザー アカウントとして設定](https://docs.microsoft.com/DeployEdge/edge-default-browser)しますか?
- レガシ バージョンの Microsoft Edge を非表示にしますか? それとも、[ユーザーが引き続き使用できるようにします](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)か?
- [Microsoft Edge の構成方法](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)。
- 初期展開の一環として、構成する上で重要な機能は何ですか?
- 特定された互換性や構成の問題に対処するためのプロセス
3. 次のような、使用する機能の前提条件を理解します。
- [Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [Internet Explorer モード](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [認証と同期](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

これらの手順を完了したら、展開戦略の計画を開始する準備が整います。
