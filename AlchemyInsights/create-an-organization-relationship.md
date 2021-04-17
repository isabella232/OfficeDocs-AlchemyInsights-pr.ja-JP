---
title: 組織の関係を作成して、ユーザーが他の組織と共同作業を行うことができるようにする
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
- "3800014"
- "898"
ms.openlocfilehash: b595fb87e18a055a7df1ff4c782a93591dd1f024
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816133"
---
# <a name="create-an-organization-relationship-to-allow-your-users-to-collaborate-with-another-organization"></a>組織の関係を作成して、ユーザーが他の組織と共同作業を行うことができるようにする

1. Microsoft 365 管理センターのダッシュボードから、**[管理者]** > **[Exchange]** の順に移動します。
2. **[組織]** > **[共有]** の順に移動します。
3. **[組織の共有]** の下の **[新規作成]** をクリックします。
4. 
            **[組織上の関係の新規作成]** の **[関係の名前]** ボックスに、組織上の関係のフレンドリ名を入力します。
5. **[共有するドメイン]** ボックスに、こちらの予定表を参照できるようにする外部の Office 365 または Exchange 社内組織のドメインを入力します。複数のドメインを入力する必要がある場合は、各ドメイン名をコンマで区切ります。たとえば、 contoso.com、service.contoso.com のようにします。
6. **[予定表の空き時間情報の共有を有効にする]** チェック ボックスを選択して、指定したドメインとの予定表の共有をオンにします。予定表の空き時間情報の共有レベルと、予定表の空き時間情報を共有できるユーザーを設定します。  

空き時間情報のアクセス レベルを設定するには、次のいずれかを選択します。

- **[時刻のみを指定して予定表の空き時間情報にアクセス]**
- **[予定表の空き時間情報のうち、空き時間、件名、場所情報へのアクセス]**  

 予定表の空き時間情報を共有する内部ユーザーを設定するには、次のいずれかを選択します。

- **組織内のすべてのユーザー**
- **[指定したセキュリティ グループ]**  


            **[参照]** をクリックし、一覧からセキュリティ グループを選択して、**[OK]** をクリックします。


            **[保存]** をクリックして組織上の関係を作成します。  

**注:** クロステナント構成は、空き時間情報の参照の個人用連絡先をサポートしていません。 空き時間情報の参照を機能させるには、連絡先をグローバル アドレス一覧に含める必要があります。

**このトピックを完全に理解するためには、以下をお読みください。**

- [Exchange Online で組織の関係を作成する](https://docs.microsoft.com/exchange/sharing/organization-relationships/create-an-organization-relationship)
- [Exchange Online での組織の関係の変更](https://docs.microsoft.com/exchange/sharing/organization-relationships/modify-an-organization-relationship)
- [Exchange Online で組織の関係を削除する](https://docs.microsoft.com/exchange/sharing/organization-relationships/remove-an-organization-relationship)
