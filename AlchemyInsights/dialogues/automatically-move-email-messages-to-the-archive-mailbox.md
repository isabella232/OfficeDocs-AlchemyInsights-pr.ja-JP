---
title: アーカイブ メールボックスへのメール メッセージの自動的な移動
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527953"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>アーカイブ メールボックスへのメール メッセージの自動的な移動

ここでは、ユーザーの古いメールを自動的にアーカイブ メールボックスに移動させるポリシーを設定する方法をご紹介します。

1. [**[セキュリティとコンプライアンス]**、](https://go.microsoft.com/fwlink/p/?linkid=2077143) > **[データガバナンス]**、 > **[アーカイブ]** の順に移動して、アーカイブ メールボックスが有効になっていることを確認します。 有効になっていない場合は、警告ボックスの **[無効化]** をクリックし、**[はい]** をクリックします。
2. [**[Exchange 管理センター]、[コンプライアンス管理]、[保持タグ]**](https://go.microsoft.com/fwlink/?linkid=2059104) の順に移動します。
3. [+] アイコンを選択し、**メールボックス全体に自動適用** を選択します。
4. 保持タグに名前を割り当て、**アーカイブに移動** を選択します。 保持期間には、90 日などの希望する期間を入力します。 **[保存]** をクリックします。
5. これで、**アイテム保持ポリシー** を選択し、アイコンを選択して新しいポリシーを追加します。
6. 保持ポリシーに名前を割り当て、クリックしてスクロールして、先ほど作成した保持タグを検出して追加します。 **[保存]** をクリックします。
7. 最後に、ユーザーのメールボックスにアイテム保持ポリシーを適用します。まだ Exchange 管理センターにいる場合は、**[受信者]**、 > **[メールボックス]** の順に移動します。 ポリシーを適用したいユーザーをすべて選択し、**[編集]** を選択します (鉛筆のアイコン)。
8. ダイアログ ボックスで、**[メールボックスの機能]** をクリックします。 **[アイテム保持ポリシー]** で、今作成したポリシーを適用して、**[保存]** します。
9. すべてのユーザーにポリシーを適用する方法については、「[メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)」参照してください。
