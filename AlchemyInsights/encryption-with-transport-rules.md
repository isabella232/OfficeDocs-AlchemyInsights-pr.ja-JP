---
title: トランスポート ルールを使用した暗号化
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5154"
ms.openlocfilehash: e1f8227047daede71d0fa3b3557db0d95a379b99b76ab0c2fe1d6ed8cc213d4a
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079455"
---
# <a name="encryption-with-transport-rules"></a>トランスポート ルールを使用した暗号化

[Exchange 管理センター](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) では、メール フロー ルールで Office Message Encryption (OME) 機能を使用して、メッセージの暗号化をトリガーできます。 トランスポート ルールの条件で、**[Office 365 Message Encryption および権利保護を適用する]** オプションを選択します。

- 詳細については、「[暗号化するためのメールフロー ルールを定義する](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)」を参照してください。

- Powershell で、[New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities) コマンドレットを使用して、"*ApplyOME*" パラメーターを $true に設定します。
