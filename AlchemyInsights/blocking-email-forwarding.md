---
title: 726 メールの転送のブロック
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
ms.openlocfilehash: 0bff7ede02809e133dc6616452ec840f552bd4fa6c45b7987d6455b2a9ba49bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54059637"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>メールの転送のブロックやブロック解除

特定のメールボックスのメールの転送を有効または無効にするには、「[メール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。

テナント レベルでは、外部転送の制御は送信スパム ポリシーを使用して行われます。 送信スパム フィルター ポリシーは、セキュリティ/コンプライアンス センターの[ここ](https://protection.office.com/antispam)から、または [Get-HostedOutboundSpamFilterPolicy コマンド](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)を使用して確認できます。

次のエラーが発生する場合: **「550 5.7.520 アクセスが拒否されました。組織は外部転送を許可していません」**。ポリシーが外部自動転送を有効にするように構成されていることを確認してください。

**注:** 既定の送信迷惑メール フィルター ポリシーで外部自動転送を無効にしておき、外部転送を必要とするユーザーにのみカスタム ポリシーを作成して外部転送を有効にすることをお勧めします。 詳細については、「[Office 365 での外部メール転送の構成](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)」を参照してください。