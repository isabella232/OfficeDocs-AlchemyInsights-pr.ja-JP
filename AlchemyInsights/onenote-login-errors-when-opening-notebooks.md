---
title: OneNote - ノートブックを開くとログイン エラーが発生する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
localization_priority: Normal
ROBOTS: NOINDEX, NOFOLLOW
ms.custom:
- "2651"
- "9000669"
ms.openlocfilehash: c928e29d931b9deb3598377864265f9e03e5ed14
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729300"
---
# <a name="issues-signing-in-to-onenote-notebooks"></a>OneNote ノートブックへのサインインの問題

ノートブックを開こうとするときに、ログインまたはパスワードのエラーが表示される場合は、次の操作を行います。

- 開けないノートブックが OneDrive または SharePoint Online に格納されている場合は、Web 用 OneNote (www.onenote.com) のノートブックが開くか試します。 ノートブックが一覧に表示されない場合は、ノートブックへのアクセス許可がない可能性があります。 共有ノートブックの場合は、所有者に共有するよう依頼して、正しいアカウントを使用してログインしていることを確認します。

- Web 用 OneNote でノートブックが開く場合は、OneNote の現在の資格情報でログインしていることを確認します。 

- [Windows 資格情報マネージャー](https://support.microsoft.com/help/4026814/windows-accessing-credential-manager)を使用して、[Office の資格情報](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) をクリアします。

- OneNote 2016 で、[**ファイル**] > [**アカウント**] の順に選択し、すべてのアカウントから [**サインアウト**] を選択します。 ライセンスが有効なユーザー アカウントを使用して、もう一度サインインします。 詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。

- OneNote for Windows で画面右上の省略記号 (**…**) を選択し、[**設定**] > [**アカウント**] の順に選択して、職場または学校のアカウントが一覧表示されていることを確認します。