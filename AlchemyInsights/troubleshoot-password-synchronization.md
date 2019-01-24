---
title: パスワード同期のトラブルシューティングを行う
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29477038"
---
# <a name="troubleshoot-password-synchronization"></a>パスワード同期のトラブルシューティングを行う

パスワードがないと Azure AD 接続バージョン 1.1.614.0 の同期またはそれ以降の問題をトラブルシューティングするには。
  
1. **管理者として実行**オプションを使用して、Azure AD 接続サーバー上の新しい Windows PowerShell セッションを開きます。 
    
2. **セット ExecutionPolicy RemoteSigned**または**無制限に設定 ExecutionPolicy**を実行します。 
    
3. Azure AD 接続ウィザードを起動します。
    
4. 移動、* * 追加のタスク * * ページで、[* * トラブルシューティング * *、[**次へ**] をクリックします。 
    
5. [トラブルシューティング] ページで、PowerShell での**トラブルシューティングを開始するのには起動**メニューをクリックします。 
    
6. メイン メニューでは、**パスワード同期のトラブルシューティングを行う**を選択します。 
    
7. サブ ・ メニューには、**パスワード同期がまったく動作しない**を選択します。 
    
 **トラブルシューティングのタスクの結果を理解します。**
  
トラブルシューティングのタスクには、次のチェックが実行されます。
  
- Azure AD テナントのパスワード同期機能が有効になっていることを検証します。
    
- Azure AD 接続サーバーはステージング モードでないことを検証します。
    
- 各既存のオンプレミス Active Directory コネクタ (これは、既存の Active Directory フォレストに相当します)。
    
- 
  - パスワード同期機能が有効になっていることを検証します。
    
  - Windows アプリケーション イベント ログ内のパスワード同期パルス イベントを検索します。
    
  - : オンプレミスの Active Directory コネクタの下にある Active Directory ドメインごとに
    
  - ドメインは、Azure AD 接続サーバーから到達できることを検証します。
    
  - オンプレミスの Active Directory コネクタが使用する Active Directory ドメイン サービス (AD DS) アカウントが正しいユーザー名、パスワード、およびパスワード同期に必要なアクセス許可を持つことを検証します。
    
パスワード同期のトラブルシューティングの詳細については、 [Azure AD 接続の同期がパスワード同期のトラブルシューティング](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization)を参照してください。
  

