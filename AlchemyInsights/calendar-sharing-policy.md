---
title: 618 予定表の共有ポリシー
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684235"
---
# <a name="policy-error-when-sharing-a-calendar"></a>予定表を共有する場合のポリシー エラー

1. 状況に応じて、次のいずれかを実行します。
    - リモート PowerShell を使用して Exchange Online に接続します。 詳細については、「[リモート PowerShell による Exchange への接続](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)」を参照してください。
    - オンプレミスのサーバーで Exchange 管理シェルを開きます。
2. ユーザーに割り当てられている共有ポリシーを決定します。 これを行うには、次のコマンドを実行して、返されたポリシーを確認します。

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. ユーザーの共有ポリシーを更新します。 これを行うには、次の手順を実行します。
    - Exchange 管理センターを開きます。
    - [**組織**] をクリックし、[**個別共有**] でユーザーに割り当てられているポリシーをダブルクリックします。 これは、手順 2 で返されたポリシーです。
    - [共有ルール] ページの [**共有する情報を指定します**] で、許可する予定表の共有レベルを選択します。[**保存**] をクリックします。

予定表を共有しようとしているときに、詳細情報については、「[このレベルのアクセス権限を 1 人以上の受信者に付与することは、ポリシーで許可されていません](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)」エラーを参照してください。
