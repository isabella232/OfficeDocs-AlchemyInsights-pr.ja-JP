---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1083"
- "3100008"
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: ce52df446fc4c23c06476e8836ade6a6810d158f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36549008"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="08e75-102">アーカイブ メールボックスへのメールの移動</span><span class="sxs-lookup"><span data-stu-id="08e75-102">Move email messages to the Archive mailbox</span></span>

1. <span data-ttu-id="08e75-103">**アーカイブ メールボックス** が有効であることを確認します。</span><span class="sxs-lookup"><span data-stu-id="08e75-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="08e75-104">有効でない場合は、[この項目](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) の手順に従いアーカイブ メールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="08e75-104">Confirm that an Archive mailbox has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="08e75-105">アーカイブ メールボックスにメッセージを自動的にアーカイブするには、保持タグと**アーカイブに移動** アクションが**自動的にメールボックス (デフォルト) タグ全体に適用する**に設定されてなければなりません。</span><span class="sxs-lookup"><span data-stu-id="08e75-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="08e75-106">タグを作成するには: [デフォルト タグをアーカイブする](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)の手順に従ってください。</span><span class="sxs-lookup"><span data-stu-id="08e75-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>

3. <span data-ttu-id="08e75-107">次に、**アーカイブ** タグを保持ポリシーに追加します。</span><span class="sxs-lookup"><span data-stu-id="08e75-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="08e75-108">Exchange 管理センターで、**保持ポリシー** を選択し、> **アーカイブ タグへ移動する**をポリシーに追加し、> **保存**を選択します。</span><span class="sxs-lookup"><span data-stu-id="08e75-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span>

4. <span data-ttu-id="08e75-109">特定のユーザーのメールボックスに[保持ポリシーを指定します](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)。</span><span class="sxs-lookup"><span data-stu-id="08e75-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="08e75-110">同じポリシーが **プライマリ** と **アーカイブ** メールボックスの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="08e75-110">Assign the Retention Policy to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span>

<span data-ttu-id="08e75-111">管理フォルダー アシスタント (MFA) を強制的に実行し、ユーザー メールボックスに新しい設定を適用させる必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="08e75-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="08e75-112">[EXO PowerShell に接続](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) されている間、次のコマンドを実行し、管理フォルダー アシスタントを特定のメールボックスで開始します。</span><span class="sxs-lookup"><span data-stu-id="08e75-112">[Solution:](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
  
<span data-ttu-id="08e75-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span><span class="sxs-lookup"><span data-stu-id="08e75-113">Start-ManagedFolderAssistant -Identity <name of the mailbox></span></span>

<span data-ttu-id="08e75-114">アーカイブ ポリシーの設定についての詳細は、[メールボックスのアーカイブの設定と削除ポリシー](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)を参照ください。</span><span class="sxs-lookup"><span data-stu-id="08e75-114">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  