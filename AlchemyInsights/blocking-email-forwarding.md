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
# <a name="blocking-or-unblocking-email-forwarding"></a><span data-ttu-id="d09e9-102">メールの転送のブロックやブロック解除</span><span class="sxs-lookup"><span data-stu-id="d09e9-102">Blocking or unblocking email forwarding</span></span>

<span data-ttu-id="d09e9-103">特定のメールボックスのメールの転送を有効または無効にするには、「[メール転送を構成する](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d09e9-103">To enable or disable email forwarding for a specific mailbox, see [Configure email forwarding](https://docs.microsoft.com/microsoft-365/admin/email/configure-email-forwarding).</span></span>

<span data-ttu-id="d09e9-104">テナント レベルでは、外部転送の制御は送信迷惑メール対策ポリシーを使用して行われます。</span><span class="sxs-lookup"><span data-stu-id="d09e9-104">On the tenant level, control of External forwarding is done using the outbound anti-spam policy.</span></span> <span data-ttu-id="d09e9-105">オフまたは自動に設定されている場合、“550 5.7.520 アクセスが拒否されました。組織では外部転送を許可していません“ エラーによりメールの転送をブロックする可能性があります。</span><span class="sxs-lookup"><span data-stu-id="d09e9-105">If it is set to Off or Automatic, it might block email forwarding with the “550 5.7.520 Access denied, Your organization does not allow external forwarding” error.</span></span> <span data-ttu-id="d09e9-106">その後、転送がブロックされるように設定されている場合には、そのエラーがユーザーに対して表示されるエラーとなります。</span><span class="sxs-lookup"><span data-stu-id="d09e9-106">Subsequently, if forwarding was set to be blocked, that is the error your users will see.</span></span>

<span data-ttu-id="d09e9-107">転送がブロックされている場合は、ポリシーが外部自動転送を有効にするように構成されていることをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="d09e9-107">If forwarding is being blocked, please make sure the policy is configured to enable External Autoforward.</span></span> <span data-ttu-id="d09e9-108">送信迷惑メール フィルター ポリシーは、セキュリティ/コンプライアンス センターから確認するか、コマンド Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode を実行することで確認することができます。</span><span class="sxs-lookup"><span data-stu-id="d09e9-108">You can check the Outbound Spam Filter Policy from Security and Compliance Center or by running command Get-HostedOutboundSpamFilterPolicy | fl name,AutoForwardingMode.</span></span> <span data-ttu-id="d09e9-109">自動転送のブロックを設定する場合は、同じコマンドで現在のポリシーの状態を確認することができます。</span><span class="sxs-lookup"><span data-stu-id="d09e9-109">If you want to set up Autoforward blocking, the same command will tell you the state of policy now.</span></span>

<span data-ttu-id="d09e9-110">注: 既定の送信迷惑メール フィルター ポリシーで外部自動転送を無効にしておき、外部転送を必要とするユーザーにのみカスタム ポリシーを作成して外部転送を有効にすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="d09e9-110">Note: It is recommended to keep the External Autoforward disabled on your Default Outbound Spam Filter Policy and enable it only for the users who need external forwarding by creating a custom policy for those users.</span></span> <span data-ttu-id="d09e9-111">詳細については、「[Configuring external email forwarding in Office 365 (Office 365 での外部メール転送の構成)](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d09e9-111">You can read more in [Configuring external email forwarding in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/external-email-forwarding).</span></span>