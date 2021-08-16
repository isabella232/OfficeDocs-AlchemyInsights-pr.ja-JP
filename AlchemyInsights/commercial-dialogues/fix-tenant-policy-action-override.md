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
ms.openlocfilehash: 9c0b88c1ca2120acccd9cd75eb918a81bde52ec3919f6148922f077f07899da7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034939"
---
# <a name="fix-tenant-policy-action-override"></a>テナント ポリシーを修正 (アクションの上書き)

テナントの迷惑メール対策ポリシーがこのメッセージに影響を与えました。 ポリシーを確認するには、次の操作を行います。

1. [Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)に移動し、**[脅威の管理]** > **[ポリシー]** > [[スパム対策]](https://go.microsoft.com/fwlink/?linkid=2101518) の順に移動します。
2. **ポリシー ソース** で以下が表示されているかどうかを確認します:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**

    その場合は、**[カスタム]** で、メッセージに影響を与えたポリシーの設定を確認します。 すべての Exchange Online Protection のユーザーに適用された **標準設定** によってメッセージが影響された可能性があります。

迷惑メール フィルター ポリシーの構成の詳細については、「[迷惑メール フィルター ポリシーを構成する](https://go.microsoft.com/fwlink/?linkid=2101431)」を参照してください。
