---
title: パブリック フォルダーの移行が 95% で失敗する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "639"
- "3500007"
ms.openlocfilehash: b22dce778b4507e0a3337a59a55531ce248b59c4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804399"
---
# <a name="public-folder-migration-fails-at-95"></a>パブリック フォルダーの移行が 95% で失敗する

移行バッチの完了を開始した可能性があり、移行バッチの状態が非常に長い間 [**同期済み**] と表示され続けます。 これは想定された動作です。

移行バッチの状態は、[**完了**] に切り替わる前に数時間 [**同期済み**] のままになるのが一般的です。 多数のターゲット メールボックスを含む移行の場合、基になるパブリック フォルダーの移行の要求が失敗または検疫されていない限り、状態は 24 時間以上 [同期済み] 状態のままです。 移行バッチがタスクを完了するまでに 24 - 48 時間かかります。

パブリック フォルダーの移行が 95% で失敗し、エラー FailedToMailEnablePublicFoldersException が発生する場合:

1. Exchange オンプレミス サーバーで [ValidateMailEnabledPublicFolders](https://aka.ms/ValidateMEPF) スクリプトをダウンロードして実行します。

2. スクリプトによって提案された修正操作を実行します。

3. Sync-MailPublicFolders (Exchange 2010 の場合) または Sync-ModernMailPublicFolders (Exchange 2013 以降の場合) を実行します。

4. パブリック フォルダーの移行を開始します。
