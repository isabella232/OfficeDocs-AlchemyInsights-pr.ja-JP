---
title: テナント ポリシーを修正 (アクションの上書き)
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
- "9000760"
- "7391"
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326802"
---
# <a name="fix-tenant-policy-action-override"></a>テナント ポリシーを修正 (アクションの上書き)

スパム対策ポリシーの 1 つが、このメッセージに影響を与えました。 ポリシーを確認するには、次の手順を実行します。

1. [ポリシー] Microsoft 365 Defenderで、[ポリシー] セクションの [&ルール脅威ポリシー&スパム対策ポリシーを電子メールで送信する] <https://security.microsoft.com/>  \>  \>  \> **に移動** します。

   **[スパム対策ポリシー]** ページに直接移動するには、<https://security.microsoft.com/antispam> を使用します。

2. [スパム **対策ポリシー** ] ページで、ポリシーの名前をクリックしてポリシーを選択します **([** 種類]は [カスタムスパム対策ポリシー] または [**名前** はスパム対策受信ポリシー **(既定)]** です)。
3. 表示される詳細フライアウトで、[アクション] セクション **の [アクションの編集** ] **を選択** します。
4. [**メッセージアクション]** セクションで、スパム、高信頼スパム、フィッシング、および高信頼フィッシングの評決を確認して、次の値が選択されている場合を確認します。 
   - **X ヘッダーの追加**
   - **件名の先頭にテキストを追加する**
   - **メッセージを電子メール アドレスにリダイレクトする**
   - **メッセージを削除する**
   - **アクションなし**

   すべての Exchange Online Protection のユーザーに適用された **標準設定** によってメッセージが影響された可能性があります。

詳細については、「[EOP でのスパム対策ポリシーの構成](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)」を参照してください。
