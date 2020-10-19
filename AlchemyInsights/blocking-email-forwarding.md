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
ms.openlocfilehash: 610013c4f46e999f1a8715aea14dd557ed8b0e2a
ms.sourcegitcommit: 88f24bb6ced16842de165af416e3f21feae13063
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/15/2020
ms.locfileid: "48478333"
---
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="b0329-102">メールの転送のブロックやブロック解除</span><span class="sxs-lookup"><span data-stu-id="b0329-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="b0329-103">特定のメールボックスのメールの転送を有効または無効にするには、「[メール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0329-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="b0329-104">テナント レベルでは、外部転送の制御は送信スパム ポリシーを使用して行われます。</span><span class="sxs-lookup"><span data-stu-id="b0329-104">On the tenant level, control of external forwarding is done using the outbound spam policy.</span></span> <span data-ttu-id="b0329-105">送信スパム フィルター ポリシーは、セキュリティ/コンプライアンス センターの[ここ](https://protection.office.com/antispam)から、または [Get-HostedOutboundSpamFilterPolicy コマンド](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy)を使用して確認できます。</span><span class="sxs-lookup"><span data-stu-id="b0329-105">You can check the outbound spam filter policy from Security and Compliance Center [here](https://protection.office.com/antispam) or by using the [Get-HostedOutboundSpamFilterPolicy command](https://docs.microsoft.com/powershell/module/exchange/get-hostedoutboundspamfilterpolicy).</span></span>

<span data-ttu-id="b0329-106">次のエラーが発生する場合: **「550 5.7.520 アクセスが拒否されました。組織は外部転送を許可していません」**。ポリシーが外部自動転送を有効にするように構成されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="b0329-106">If you are getting the following error: **“550 5.7.520 Access denied, Your organization does not allow external forwarding”**, please make sure the policy is configured to enable External Auto-forward.</span></span>

<span data-ttu-id="b0329-107">**注:** 既定の送信迷惑メール フィルター ポリシーで外部自動転送を無効にしておき、外部転送を必要とするユーザーにのみカスタム ポリシーを作成して外部転送を有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b0329-107">**Note:** It is recommended to keep the External Autoforward disabled on your default outbound spam filter policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="b0329-108">詳細については、「[Office 365 での外部メール転送の構成](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0329-108">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>