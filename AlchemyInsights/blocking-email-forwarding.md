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
ms.openlocfilehash: c0d9ed14f83d3c7d47e1728d5ed9ca3a19412ad2
ms.sourcegitcommit: f74c9698a31634154ce58dda8b3145bb10685ace
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/23/2020
ms.locfileid: "48219860"
---
# <a name="blocking-or-unblocking-email-forwarding"></a>メールの転送のブロックやブロック解除

特定のメールボックスのメールの転送を有効または無効にするには、「[メール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。

テナント レベルでは、外部転送の制御は送信迷惑メール対策ポリシーを使用して行われます。 オフまたは自動に設定されている場合、“550 5.7.520 アクセスが拒否されました。組織では外部転送を許可していません“ エラーによりメールの転送をブロックする可能性があります。 その後、転送がブロックされるように設定されている場合には、そのエラーがユーザーに対して表示されるエラーとなります。

転送がブロックされている場合は、ポリシーが外部自動転送を有効にするように構成されていることをご確認ください。 送信迷惑メール フィルター ポリシーは、セキュリティ/コンプライアンス センターから確認するか、コマンド Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode を実行することで確認することができます。 自動転送のブロックを設定する場合は、同じコマンドで現在のポリシーの状態を確認することができます。

注: 既定の送信迷惑メール フィルター ポリシーで外部自動転送を無効にしておき、外部転送を必要とするユーザーにのみカスタム ポリシーを作成して外部転送を有効にすることをお勧めします。 詳細については、「[Configuring external email forwarding in Office 365 (Office 365 での外部メール転送の構成)](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)」を参照してください。