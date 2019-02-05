---
title: アーカイブ メールボックスへのメール メッセージの移動
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 59cd8630-6196-4680-ad92-1ce0e479f924
ms.openlocfilehash: 2147c70f64087bf95fc4e39c193caeac3b2c5361
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29660387"
---
<span data-ttu-id="7160d-p101">アーカイブ メールボックスにアイテムを整理すると、問題が発生します。次の手順を実行したことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="7160d-p101">Having problems archiving items to the Archive mailbox. Make sure you have performed the following steps:</span></span>
  
1. <span data-ttu-id="7160d-p102">**[アーカイブ メールボックス]** が有効になっていることを確認します。そうでない場合は、[この記事](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes)の手順を使用して、アーカイブ メールボックスを有効にします。</span><span class="sxs-lookup"><span data-stu-id="7160d-p102">Confirm that an **Archive mailbox** has been enabled. If not, use steps in [this article](https://docs.microsoft.com/office365/securitycompliance/enable-archive-mailboxes) to enable the archive mailbox.</span></span> 
    
2. <span data-ttu-id="7160d-106">Exchange 管理センターで、**[コンプライアンス管理]** の下の **[保持タグ]** を選択し、必要な**保存の有効期限**を含む **[アーカイブに移動]** アクションを使用した**保持タグ**を作成します。</span><span class="sxs-lookup"><span data-stu-id="7160d-106">In the Exchange Admin Center, select **Retention Tags** under **Compliance Management**, create a **Retention tag** with the **Move to Archive** action containing the desired **Retention Age**.</span></span>
    
3. <span data-ttu-id="7160d-107">Exchange 管理センターで、**[アイテム保持ポリシー]** を選択し、**[アイテム保持ポリシー]** を作成し、そのポリシーに **[アーカイブに移動]** 保持タグを追加します。</span><span class="sxs-lookup"><span data-stu-id="7160d-107">In the Exchange Admin Center, select **Retention Policies**, create a **Retention Policy** and add your **Move to Archive** retention tag to that policy.</span></span> 
    
4. <span data-ttu-id="7160d-p103">特定のユーザーのメールボックスに[アイテム保持ポリシーを割り当て](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)ます。同じポリシーは、**プライマリ**および**アーカイブ** メールボックスにも適用されます。</span><span class="sxs-lookup"><span data-stu-id="7160d-p103">[Assign the Retention Policy](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) to the specific user's mailbox. The same policy will be applied to both the **Primary** and the **Archive** mailbox.</span></span> 
    
<span data-ttu-id="7160d-p104">これでユーザーのメールボックスには、アイテムをアーカイブ メールボックスに移動するアーカイブ ポリシーが用意されました。場合によっては、強制的に管理フォルダー用アシスタント (MFA) を実行して、新しい設定をユーザーのメールボックスに適用する必要があります。[EXO PowerShell に接続された](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)状態で次のコマンドを実行し、特定のメールボックスに対して管理フォルダー用アシスタントを起動します。</span><span class="sxs-lookup"><span data-stu-id="7160d-p104">The user's mailbox should now have an Archive policy to move items to the Archive mailbox. It may be necessary to force the Managed Folder Assistant (MFA) to run and apply the new settings to the user's mailbox. Run the following command while [connected to EXO PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) to start the Managed Folder Assistant for a specific mailbox:</span></span> 
  
```
Start-ManagedFolderAssistant -Identity <name of the mailbox>
```

<span data-ttu-id="7160d-113">アーカイブ ポリシーの設定の詳細については、[メールボックスのアーカイブと削除ポリシーの設定](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="7160d-113">Want more information on setting up an archive policy, see [Set up an archive and deletion policy for mailboxes](https://docs.microsoft.com/office365/securitycompliance/set-up-an-archive-and-deletion-policy-for-mailboxes#step-1-enable-archive-mailboxes-for-users).</span></span>
  

