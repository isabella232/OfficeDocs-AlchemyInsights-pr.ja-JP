---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 35c11f1bfb7c61b28a64f0128c29ddf7b4fce939
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511045"
---
# <a name="move-email-to-the-archive-mailbox"></a>アーカイブ メールボックスへのメールの移動

1. **アーカイブ メールボックス** が有効であることを確認します。 有効でない場合は、[この項目](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) の手順に従いアーカイブ メールボックスを有効にします。

2. アーカイブ メールボックスにメッセージを自動的にアーカイブするには、保持タグと**アーカイブに移動** アクションが**自動的にメールボックス (デフォルト) タグ全体に適用する**に設定されてなければなりません。 タグを作成するには: [デフォルト タグをアーカイブする](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)の手順に従ってください。

3. 次に、**アーカイブ** タグを保持ポリシーに追加します。 Exchange 管理センターで、**保持ポリシー** を選択し、> **アーカイブ タグへ移動する**をポリシーに追加し、> **保存**を選択します。

4. 特定のユーザーのメールボックスに[保持ポリシーを指定します](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。 同じポリシーが **プライマリ** と **アーカイブ** メールボックスの両方に適用されます。

管理フォルダー アシスタント (MFA) を強制的に実行し、ユーザー メールボックスに新しい設定を適用させる必要がある場合があります。 [EXO PowerShell に接続](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) されている間、次のコマンドを実行し、管理フォルダー アシスタントを特定のメールボックスで開始します。
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

アーカイブ ポリシーの設定についての詳細は、[メールボックスのアーカイブの設定と削除ポリシー](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)を参照ください。
  