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
ms.openlocfilehash: 59360a040fe413e92cd880b1225b9006384a823f6e8abeb7ef922949b9a874fd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035227"
---
# <a name="configure-message-encryption-for-a-hybrid-environment"></a>ハイブリッド環境でのメッセージ暗号化の構成

ハイブリッド Exchange 環境の場合、オンプレミスのユーザーは、メールが Exchange Online 経由でルーティングされている場合に限り、Office Message Encryption (OME) を使用して暗号化されたメールを送信することができます。

OME を使用してメールを暗号化するには、以下の手順を実行します。

1. [ハイブリッド構成ウィザード](https://docs.microsoft.com/Exchange/hybrid-configuration-wizard)を使用して、ハイブリッド環境を設定します。 暗号化の設定に特別な手順は必要ありません。
2. 通常行っているように[暗号化のためのメール フロー ルールを設定します](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)。


