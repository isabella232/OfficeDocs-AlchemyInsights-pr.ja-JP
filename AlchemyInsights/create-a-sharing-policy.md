---
title: 共有ポリシーを作成して、ユーザーが自分の予定表を組織外のユーザーと共有できるようにする
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 9ece122e0905d1afeb26e50fa0a5e049eee5c09d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806728"
---
# <a name="create-a-sharing-policy-to-allow-your-users-to-share-their-calendar-with-people-outside-your-organization"></a>共有ポリシーを作成して、ユーザーが自分の予定表を組織外のユーザーと共有できるようにする

1. Microsoft 365 管理センターのダッシュボードから、**[管理者]** > **[Exchange]** の順に移動します。
2. **[組織]** > **[共有]** の順に移動します。
3. リスト ビューの **[個別共有]** で、**[新規作成]** をクリックします。
4. **[共有ポリシーの新規作成]** で、**[ポリシー名]** ボックスに共有ポリシーのフレンドリ名を入力します。
5. **[追加]** をクリックして、ポリシーの共有ルールを定義します。
6. 
            **[共有ルール]** で、次のいずれかのオプションを選択して、共有するドメインを指定します。
    - **[すべてのドメインと共有]**
    - **[特定のドメインと共有]**
8. 
            **[特定のドメインと共有]** を選択した場合は、共有するドメインの名前を入力します。この共有ポリシーに複数のドメインを入力する必要がある場合は、最初のドメインの設定値を保存してから、共有ルールを編集してさらにドメインを追加します。
9. 共有できる情報を指定するには、**[予定表フォルダーを共有する]** チェック ボックスを選択してから、以下のいずれかのオプションを選択します。
    - **[時刻のみを指定して予定表の空き時間情報にアクセス]**
    - **[時間、件名、場所を含む予定表の空き時間情報]**
    - **[時刻、件名、場所、役職などの予定表のすべての予定情報]**
11. 共有ポリシーのルールを設定するには、**[保存]** をクリックします。
12. この共有ポリシーを組織内のすべてのユーザーの新しい既定の共有ポリシーに設定するには、 **[このポリシーを既定の共有ポリシーにする]** チェック ボックスをオンにします。
13. **[保存]** をクリックして、共有ポリシーを作成します。  

**このトピックを完全に理解するためには、以下をお読みください。**

- [Exchange Online で共有ポリシーを作成する](https://docs.microsoft.com/exchange/sharing/sharing-policies/create-a-sharing-policy)
- [Exchange Online で共有ポリシーをメールボックスに適用する](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy)
- [Exchange Online での共有ポリシーの変更、無効化、削除](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)