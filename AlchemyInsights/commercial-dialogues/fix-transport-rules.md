---
title: トランスポート ルールを修正する
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751415"
---
# <a name="fix-transport-rules"></a>トランスポート ルールを修正する

カスタムのメール フロー ルールがこのメッセージに影響を与えました。 正確なルールを確認するには、次の手順を実行します。

1. 送信結果の **[追加情報]** で、**GUID** または **ポリシー名** を確認します。
2. Exchange 管理シェルを起動します。 詳細については、「[Exchange 管理シェルを開く](https://go.microsoft.com/fwlink/?linkid=2101432)」を参照してください。
3. (送信時の GUID を使用して) 次のコマンドを実行します: **Get-TransportRule -identity "GUID" | fl * Description***
4. 説明を確認して、メッセージに影響を与えた構成済みの条件を確認します。

詳細については、「[Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523)」を参照してください。
