---
title: macOS 11.6 Big Sur にアップグレードした後にアカウントを追加できない
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: 91cb402e63b68de4a08f6dcb80807ff2e01300c9
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506146"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>macOS 11.6 Big Sur にアップグレードした後にアカウントを追加できない

macOS 11.6 にアップグレードすると、職場または学校用の OneDrive アカウントまたは OneDrive 個人用アカウントがアカウントの一覧に表示されず、アプリから 2 つ目のアカウントにログインできない可能性があります。

この問題の修正プログラムが開発されました。 まず、OneDrive のスタンドアロン バージョンと App Store バージョンのどちらを実行しているかを確認します。

- メニュー バーの **[ヘルプと設定]**  >  **[ユーザー設定]**  >  **[バージョン情報]** のメニュー バーで OneDrive クラウドを選択します。 バージョン番号に **(Standalone)** が含まれていない場合は、製品の App Store バージョンがあります。

スタンドアロン バージョンの OneDrive を使用している場合は、コンピューターを再起動すると、この問題が解決されたビルドに OneDrive が自動更新されます。 ビルドを手動でインストールする場合は、この [.zip file](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip) をダウンロードし、ファイルを解凍し、OneDrive アプリをアプリケーション フォルダーにコピーします (既存の OneDrive アプリを置き換えます)。

App Store バージョンを使用している場合は、スタンドアロン バージョンの OneDrive をインストールすることを検討してください。 このバージョンは、App Store バージョンと同じ動作をしますが、Microsoft により更新プログラムをより迅速にユーザーに提され、この問題の修正プログラムを含むバージョンに接続されます。

1. [修正プログラムを含む OneDrive](https://oneclient.sfx.ms/Mac/Prod/21.170.0822.0003/OneDrive.zip) のスタンドアロン バージョンをダウンロードします。
2. ファイルを解凍し、OneDrive アプリをアプリケーション フォルダーにコピーします (既存の OneDrive アプリを置き換えます)。

App Store バージョンを使用する必要がある場合は、App Store が修正プログラムを含むアプリのバージョンをリリースするまで待ってください。 残念ながら、Microsoft は、App Store からの固定バージョンのリリース予測日を伝えることはできません。


