---
title: ノートブックを開くときの問題を解決する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002359"
- "4718"
ms.openlocfilehash: 1015b3a82fa4e90c66ca05cf528167d0a0e120e8e6833d1b0c21948f453436b8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057071"
---
# <a name="fix-issues-with-opening-notebooks"></a>ノートブックを開くときの問題を解決する

**重要**: 次のようなメッセージが表示される場合があります。"Microsoft Teams で OneNote の制限が発生しています。 このノートブックを編集するには、OneNote for the web を使用してください。"

「[メッセージ センター ID: 207439 - Microsoft 365 の一時的な機能の調整への認識](https://admin.microsoft.com/Adminportal/Home?source=applauncher#MessageCenter?id=MC207439)」を参照してください。

Teams での OneNote は、商用および教育のテナントに対して読み取り専用になります。 編集するには、OneNote for the web または OneNote デスクトップ アプリを使用してください。

ノートブックを開くときの問題に対する一般的な解決策を次に示します。

1. 職場または学校のアカウントではなく個人アカウントでログインしているため、ノートブックを開くことができない場合があります。
    - OneNote for the web でノートブックが開く場合は、OneNote の現在の資格情報でログインしていることを確認します。
    - OneNote 2016 では、**[ファイル] > [アカウント]** の順にクリックし、すべてのアカウントで **[サインアウト]** をクリックします。 ライセンスが有効なユーザー アカウントを使用して、もう一度サインインします。 詳細については、「[Office のアカウント](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9)」を参照してください。 
    - OneNote for Windows では、画面右上の省略記号 (**…**) をクリックし、**[設定] > [アカウント]** の順にクリックして、職場または学校のアカウントが一覧表示されていることを確認します。 
2. 開けないノートブックが OneDrive または SharePoint Online に格納されている場合は、[OneNote for the web](https://onenote.com) のノートブックが開くか試します。 ノートブックが一覧に表示されない場合は、ノートブックへのアクセス許可がない可能性があります。 共有ノートブックの場合は、所有者に共有するよう依頼して、正しいアカウントを使用してログインしていることを確認します。
