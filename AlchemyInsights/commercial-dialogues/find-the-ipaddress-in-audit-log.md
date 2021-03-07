---
title: 監査ログで IP アドレスを見つける
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 7a01aa3cc0d875e6534435f3e8f90a24f2832dc3
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484150"
---
# <a name="find-the-ip-address-in-audit-log"></a>監査ログで IP アドレスを見つける

1. ユーザーまたは管理者によって実行されたアクティビティに対応する IP アドレスが監査ログに表示されます。 クライアント情報も記録されます。 IP アドレスを特定する方法は次のとおりです。

1. [Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動します。
1. **[検索]** > **[ [監査ログ検索]](https://go.microsoft.com/fwlink/?linkid=2103759)** を選択します。
    > [!NOTE]
    > 監査を有効にする必要があるという通知が表示された場合は、先に進んで今すぐ有効にしてください。 この機能が有効になっていない場合、検索結果は前の日付からデータを取得できません。
1. 特定のアクティビティに興味がある場合は、**[アクティビティ]** リストから選択してください。 それ以外の場合、既定では、選択したユーザーのすべてのアクティビティが返されます。 特定のアクティビティは、**[アクティビティ]** メニューから選択できない場合があることに注意してください。 ただし、**[すべてのアクティビティの結果を表示する]** が選択されている場合 (既定設定)、これらの監査項目が返されます。
1. 日付範囲を指定し、**[ユーザー]** フィールドで、調査するユーザーのユーザー名を選択します。
1. **[検索]** を選択します。 アクティビティは **[結果]** の下に表示されます。 各アクティビティの IP アドレスを確認できます。
1. 詳細を表示するには、アクティビティを選択してから、**[詳細情報]** を選択します。

詳細については、「[Office 365 監査ログを検索して一般的なシナリオのトラブルシューティングを行う](https://go.microsoft.com/fwlink/?linkid=2103944)」を参照してください。