---
title: 外部のメールの自動転送をブロックまたはブロックを解除する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "726"
- "1200004"
ms.assetid: 8865c68e-7e8a-4135-a254-d7f69f1ded30
ms.openlocfilehash: fe9e52023b809b38c43332a10a1184d114798cfe
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315879"
---
# <a name="block-or-unblock-eternal-automatic-email-forwarding"></a>永続的なメールの自動転送をブロックまたはブロックを解除する

特定のメールボックスのメールの転送を有効または無効にするには、「[メール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。

管理者は、[送信スパム ポリシー](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-outbound-spam-policy)を使用して、組織の外部への転送を制御できます。 送信スパム ポリシーを管理するには、<https://security.microsoft.com/antispam> の Microsoft 365 Defender ポータル、または Exchange Online PowerShell の [Get-HostedOutboundSpamFilterPolicy](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy) コマンドレットを使用します。

**「550 5.7.520 アクセスが拒否されました。組織は外部転送を許可していません」** というエラーが発生する場合は、ポリシーが外部への自動転送を有効にするように構成されているかどうかを確認してください。

**注**: 既定値である **自動 - システム既定の送信スパム フィルター ポリシーの **自動転送ルール** 設定用に制御された** システム (外部への自動転送はブロックされますが、内部への自動転送は引き続き機能する) をお勧めします。 外部へのメールの自動転送が必要なユーザーに対してのみ、カスタムの送信スパム フィルター ポリシーを作成し、**On (転送が有効)** の値を使用する必要があります。 詳細については、「[Office 365 で外部へのメール転送を構成する](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)」を参照してください。
