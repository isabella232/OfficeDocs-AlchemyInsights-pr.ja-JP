---
title: 接続 ポリシーを修正
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314849"
---
# <a name="fix-connection-policy"></a>接続 ポリシーを修正

既定の接続フィルター ポリシーで送信元 IP アドレスが安全とマークされたため、電子メールは安全とマークされ、ユーザーの受信トレイに配信されました。 ポリシーを確認するには、次の手順を実行します。

1. [ポリシー] Microsoft 365 Defenderで、[ポリシー] セクションの [&ルール脅威ポリシー&スパム対策ポリシーを電子メールで送信する] <https://security.microsoft.com/>  \>  \>  \> **に移動** します。

   **[スパム対策ポリシー]** ページに直接移動するには、<https://security.microsoft.com/antispam> を使用します。

2. [スパム **対策ポリシー]** ページで、ポリシーの名前をクリックして、接続フィルター ポリシー **(既定)** という名前のポリシーを選択します。

3. 表示される詳細フライアウトで、[ **接続フィルター]** セクションの [接続フィルター ポリシーの編集 **] をクリック** します。

4. [次の **IP** アドレスまたはアドレス範囲からのメッセージを常に許可する] セクションのエントリを確認し、[安全な一覧を有効にする] が **選択されている場合** を確認します。

   **注**: Microsoft は、信頼できる送信者のサード パーティソースにサブスクライブしています。 セーフ リストが有効になっている場合、これらの信頼できる送信者は誤ってスパムとしてマークされません。 このオプションを選択することをお勧めします。これは、受信する誤検知 (スパムに分類される良いメール) の数を減らすためです。

詳細については、「[接続フィルターを構成する](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)」を参照してください。
