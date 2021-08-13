---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 7e72766f441e210a81fcfd6c07b1801f6c0474afb02a70edf2ad8dbb571f3d2a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53974962"
---
# <a name="move-email-to-the-archive-mailbox"></a>アーカイブ メールボックスへのメールの移動

下記の設定の自動チェックを実行する場合は、このページの上部にある [戻る <--] ボタンを選択し、メールをアーカイブメールボックスに移動できないユーザーのメールアドレスを入力します。

1. **[アーカイブ メールボックス]** が有効になっていることを確認します。有効になっていない場合は、[この記事](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes)の手順を使用して、アーカイブ メールボックスを有効にします。

2. アーカイブ メールボックスにメッセージを自動的にアーカイブするには、保持タグと **アーカイブに移動** アクションが **自動的にメールボックス (デフォルト) タグ全体に適用する** に設定されてなければなりません。タグを作成するには、次の手順を使用します：[アーカイブデフォルトタグ](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)。

3. **アーカイブ** タグを保持ポリシーに追加します。Exchange 管理センターで、**保持ポリシー** を選択し、> **アーカイブ タグへ移動する** をポリシーに追加し、> **保存** を選択します。

4. 次に、特定のユーザーのメールボックスに [アイテム保持ポリシーを割り当て](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ます。同じポリシーは、**プライマリ** および **アーカイブ** メールボックスにも適用されます。

これでユーザーのメールボックスには、アイテムをアーカイブ メールボックスに移動するアーカイブ ポリシーが用意されました。場合によっては、強制的に管理フォルダー用アシスタント (MFA) を実行して、新しい設定をユーザーのメールボックスに適用する必要があります。[EXO PowerShell に接続された](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)状態で次のコマンドを実行し、特定のメールボックスに対して管理フォルダー用アシスタントを起動します。
  
Start-ManagedFolderAssistant -Identity <name of the mailbox>

アーカイブ ポリシーの設定についての詳細は、[メールボックスのアーカイブの設定と削除ポリシー](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)を参照ください。
  