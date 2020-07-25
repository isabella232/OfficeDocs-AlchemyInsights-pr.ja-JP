---
title: パスワード同期のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387882"
---
# <a name="troubleshoot-password-synchronization"></a>パスワード同期のトラブルシューティング

パスワードの同期の問題をトラブルシューティングするには、この AAD Connect のトラブルシューティングタスクを使用して、パスワードが同期されない理由を特定します。 開始するには、[直接同期を管理](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)に移動します。  

1. Azure AD Connect サーバーで新しい Windows PowerShell セッションを開いて、[**管理者として実行**] オプションを選択します。

2. Set-ExecutionPolicy RemoteSigned または Set-ExecutionPolicy Unrestricted を実行します。

3. Azure AD Connect ウィザードを開始します。

4. 追加のタスクページ ＞ **トラブルシューティング** > **次へ**の順に移動します。

5. [**起動**] を選択して、PowerShell のトラブルシューティングメニューを開きます。

6. **パスワード同期のトラブルシューティング**を選択します。

    通常、特定のユーザーアカウントのパスワードは同期されないことが問題になります。

    **注** 最後に通常にパスワードを同期してから時間が経過している場合は、パスワードを同期できません。

パスワード同期のトラブルシューティングの詳細については、「[Azure AD Connect 同期によるパスワードハッシュ同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」を参照してください。