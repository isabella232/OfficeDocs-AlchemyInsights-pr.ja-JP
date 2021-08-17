---
title: ユーザーが作成した電子メールの署名をブロックする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1200009"
- "7310"
ms.openlocfilehash: ad743cea4b8735b35b90bd5bf3d0b5b933184ed82858e828a68beb2ca2f8270c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54103557"
---
# <a name="block-user-made-email-signatures"></a>ユーザーが作成した電子メールの署名をブロックする

次の解決策は、Outlook on the Web で作成された電子メール署名にのみ適用されます。 オンプレミスの Exchange Serverが ある場合にのみ、Outlook アプリで署名をブロックできます。

1. 管理センターで、**[管理センター]** > **[Exchange]** の順に選択します。
2. **[アクセス許可]** > **[Outlook Web App ポリシー]** の順にクリックします。
3. ポリシーを選択し、鉛筆アイコンをクリックして編集します。
4. **[機能]** > **[その他のオプション]** の順にクリックします。
5. **[ユーザー エクスペリエンス]** で、**[電子メールの署名]** チェックボックスをオフにし、**[保存]** をクリックします。

**重要:** このチェックボックスをオフにする前に署名が追加された場合でも、ユーザーはその署名を使用できます。 それらを削除するように依頼してください。
