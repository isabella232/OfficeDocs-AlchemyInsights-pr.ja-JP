---
title: パスワード同期のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353110"
---
# <a name="troubleshoot-password-synchronization"></a>パスワード同期のトラブルシューティング

Azure AD Connect バージョン 1.1.614.0 以降とパスワードが同期されないという問題をトラブルシューティングするには:
  
1. [**管理者として実行**] オプションを使用して、Azure AD Connect サーバーで新しい Windows PowerShell セッションを開きます。

2. **Set-ExecutionPolicy RemoteSigned** または **Set-ExecutionPolicy Unrestricted** を実行します。

3. Azure AD Connect ウィザードを開始します。

4. **[追加のタスク]** ページに移動し、**[トラブルシューティング]** を選択して **[次へ]** をクリックします。

5. [トラブルシューティング] ページで、PowerShell の [**起動してトラブルシューティングを開始する**] メニューをクリックします。

6. メイン メニューで、[**パスワード同期のトラブルシューティング**] を選択します。

7. サブメニューで、[**パスワード同期がまったく動作しない**] を選択します。

**トラブルシューティング タスクの結果を理解する**
  
トラブルシューティング タスクでは、次のチェックが実行されます。
  
- Azure AD テナントのパスワード同期機能が有効になっていることを確認します。

- Azure AD Connect サーバーがステージング モードではないことを確認します。

- (既存の Active Directory フォレストに対応する) 既存のオンプレミス Active Directory コネクタごとに、次の手順を実行します。

- 
  - パスワード同期機能が有効になっていることを確認します。

  - Windows アプリケーション イベント ログでパスワード同期ハートビート イベントを検索します。

  - オンプレミスの Active Directory コネクタの下にある Active Directory ドメインごとに、次の手順を実行します。

  - Azure AD Connect サーバーからドメインにアクセスできることを確認します。

  - オンプレミスの Active Directory コネクタで使用される Active Directory ドメイン サービス (AD DS) アカウントに、正しいユーザー名、パスワード、およびパスワードの同期に必要なアクセス許可があることを確認します。

パスワード同期のトラブルシューティングの詳細については、「[Azure AD Connect 同期によるパスワード同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)」を参照してください。
  