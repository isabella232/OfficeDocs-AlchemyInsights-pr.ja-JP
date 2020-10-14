---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 61d0b1a58fff6655b745bb9d39e8384f0a543336
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799785"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="736f1-102">アーカイブ メールボックスへのメールの移動</span><span class="sxs-lookup"><span data-stu-id="736f1-102">Move email to the archive mailbox</span></span>

<span data-ttu-id="736f1-103">下記の設定の自動チェックを実行する場合は、このページの上部にある [戻る <--] ボタンを選択し、メールをアーカイブメールボックスに移動できないユーザーのメールアドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="736f1-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems moving email to their archive mailbox.</span></span>

1. <span data-ttu-id="736f1-104">**アーカイブ メールボックス** が有効であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="736f1-104">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="736f1-105">有効でない場合は、[この項目](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) の手順に従いアーカイブ メールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="736f1-105">If not, use the steps in [this article](https://docs.microsoft.com/microsoft-365/compliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="736f1-106">アーカイブ メールボックスにメッセージを自動的にアーカイブするには、保持タグと**アーカイブに移動** アクションが**自動的にメールボックス (デフォルト) タグ全体に適用する**に設定されてなければなりません。</span><span class="sxs-lookup"><span data-stu-id="736f1-106">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="736f1-107">タグを作成するには: [デフォルト タグをアーカイブする](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag)の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="736f1-107">Use the steps here to create the tag: [Archive Default tag](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#create-a-custom-archive-default-policy-tag).</span></span>

3. <span data-ttu-id="736f1-108">次に、**アーカイブ** タグを保持ポリシーに追加します。</span><span class="sxs-lookup"><span data-stu-id="736f1-108">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="736f1-109">Exchange 管理センターで、**保持ポリシー** を選択し、> **アーカイブ タグへ移動する**をポリシーに追加し、> **保存**を選択します。</span><span class="sxs-lookup"><span data-stu-id="736f1-109">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="736f1-110">特定のユーザーのメールボックスに[保持ポリシーを指定します](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。</span><span class="sxs-lookup"><span data-stu-id="736f1-110">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="736f1-111">同じポリシーが **プライマリ** と **アーカイブ** メールボックスの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="736f1-111">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="736f1-112">管理フォルダー アシスタント (MFA) を強制的に実行し、ユーザー メールボックスに新しい設定を適用させる必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="736f1-112">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="736f1-113">[EXO PowerShell に接続](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) されている間、次のコマンドを実行し、管理フォルダー アシスタントを特定のメールボックスで開始します。</span><span class="sxs-lookup"><span data-stu-id="736f1-113">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="736f1-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="736f1-114">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="736f1-115">アーカイブ ポリシーの設定についての詳細は、[メールボックスのアーカイブの設定と削除ポリシー](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)を参照ください。</span><span class="sxs-lookup"><span data-stu-id="736f1-115">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/microsoft-365/compliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  