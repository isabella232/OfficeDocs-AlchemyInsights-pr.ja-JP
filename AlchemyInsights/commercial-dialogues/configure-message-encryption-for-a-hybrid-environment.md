---
title: ハイブリッド環境でのメッセージ暗号化の構成
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 22c2468b7639680b447b6464431a79b69f7198c3
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751213"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>ハイブリッド環境でのメッセージ暗号化の構成

ハイブリッド Exchange 環境の場合、オンプレミスのユーザーは、メールが Exchange Online 経由でルーティングされている場合に限り、Office Message Encryption (OME) を使用して暗号化されたメールを送信することができます。

OME を使用してメールを暗号化するには、以下の手順を実行します。

1. [ハイブリッド構成ウィザード](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard)を使用して、ハイブリッド環境を設定します。 暗号化の設定に特別な手順は必要ありません。
2. 通常行っているように[暗号化のためのメール フロー ルールを設定します](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。


