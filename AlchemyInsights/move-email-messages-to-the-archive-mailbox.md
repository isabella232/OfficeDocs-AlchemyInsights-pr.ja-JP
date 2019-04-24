---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 37f256ef31402f5139fdd7c2af8f3a6ca9dc3525
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418324"
---
# <a name="move-email-to-the-archive-mailbox"></a><span data-ttu-id="ef5a1-102">メールをアーカイブメールボックスに移動する</span><span class="sxs-lookup"><span data-stu-id="ef5a1-102">Move email to the archive mailbox</span></span>
 
1. <span data-ttu-id="ef5a1-103">**アーカイブメールボックス**が有効になっていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-103">Confirm that an **Archive mailbox** has been enabled.</span></span> <span data-ttu-id="ef5a1-104">それ以外の場合は、[この記事](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)の手順を使用してアーカイブメールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-104">If not, use the steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span>

2. <span data-ttu-id="ef5a1-105">アーカイブメールボックスにメッセージを自動的にアーカイブするには、[**アーカイブに移動**する] アクションを持つ保持タグを、 **mailbox (default) タグ全体に自動的に適用**するように設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-105">To archive messages automatically to the archive mailbox, a retention tag with the **Move to archive** action must be set to **applied automatically to entire mailbox (default) tag**.</span></span> <span data-ttu-id="ef5a1-106">タグ: [Archive Default タグ](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0)を作成するには、以下の手順を使用します。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-106">Use the steps here to create the tag: [Archive Default tag](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Fen-us%2Foffice365%2Fsecuritycompliance%2Fset-up-an-archive-and-deletion-policy-for-mailboxes%23create-a-custom-archive-default-policy-tag&data=04%7C01%7Cstephow%40microsoft.com%7C89934e16dbd84ebdef6708d6b319b348%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636893320296576506%7CUnknown%7CTWFpbGZsb3d8eyJWIjoiMC4wLjAwMDAiLCJQIjoiV2luMzIiLCJBTiI6Ik1haWwiLCJXVCI6Mn0%3D%7C-1&sdata=UibWi%2BtrO3ITZ6iF%2FtKQj5JyxzEb9Mu9frBJPT6FNFI%3D&reserved=0).</span></span>
    
3. <span data-ttu-id="ef5a1-107">次に、アイテム保持ポリシーに**アーカイブ**タグを追加します。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-107">Next, add the **Archive** tag to your retention policy.</span></span> <span data-ttu-id="ef5a1-108">Exchange 管理センターで [**アイテム保持ポリシー** >] を選択し、[**アーカイブに移動する] タグ**を [ポリシー >**保存**] に追加します。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-108">In the Exchange admin center, choose **Retention Policies** > add the **Move to Archive tag** to the policy > **Save**.</span></span> 
    
4. <span data-ttu-id="ef5a1-109">次に[、アイテム保持ポリシー](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)を特定のユーザーのメールボックスに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-109">Now [Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox.</span></span> <span data-ttu-id="ef5a1-110">同じポリシーが**プライマリ**メールボックスと**アーカイブ**メールボックスの両方に適用されます。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-110">The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="ef5a1-111">管理フォルダーアシスタント (MFA) を強制的に実行して、新しい設定をユーザーのメールボックスに適用する必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-111">It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox.</span></span> <span data-ttu-id="ef5a1-112">[exo PowerShell に接続して](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)いるときに、特定のメールボックスの管理フォルダーアシスタントを開始するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-112">Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="ef5a1-113">アーカイブポリシーの設定の詳細については、「[メールボックスのアーカイブおよび削除ポリシーをセットアップする](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ef5a1-113">For more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

