---
title: 動作していない Exchange 管理センターでの保存ポリシー
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 0ceb1737040f0304bfe8b611241ce1deef487652
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/15/2019
ms.locfileid: "28297193"
---
 <span data-ttu-id="14664-102">**問題:** 新しく作成されたメールボックスに、Exchange 管理センターで最新のリテンション ・ ポリシーを適用しないまたはアイテムのアーカイブ メールボックスに移動または削除はできません。</span><span class="sxs-lookup"><span data-stu-id="14664-102">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="14664-103">**根本的な原因。**</span><span class="sxs-lookup"><span data-stu-id="14664-103">**Root Causes:**</span></span>
  
- <span data-ttu-id="14664-p101">**管理フォルダー アシスタント**は処理されないため、ユーザーのメールボックスがあります。管理フォルダー アシスタントを 7 日間に 1 回に、クラウド ベース組織内のすべてのメールボックスの処理を試みます。保持タグを変更するメールボックスに異なるアイテム保持ポリシーを適用するか、待つことができます。、メールボックスを処理する、管理フォルダーを支援または管理フォルダー アシスタントに特定の処理を開始する開始 ManagedFolderAssistant コマンドレットを実行することができます。メールボックスです。このコマンドレットを実行することがテストまたは保持ポリシーまたは保持タグ設定のトラブルシューティングに便利です。詳細については、[管理フォルダー アシスタントの実行](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14664-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/en-us/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="14664-109">**ソリューション:** 管理フォルダー アシスタントに特定のメールボックスを開始する次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="14664-109">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span> 
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="14664-p102">**RetentionHold**は、メールボックスで**有効になっている**がされている場合これも発生します。場合は、RetentionHold には、メールボックスが置かれた、その時に、メールボックスに保持ポリシーは処理されません。詳細については、RetentionHold の設定を参照してください:[メールボックスの保存を保持](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)します。</span><span class="sxs-lookup"><span data-stu-id="14664-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/en-us/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="14664-113">**ソリューション:**</span><span class="sxs-lookup"><span data-stu-id="14664-113">**Solution:**</span></span>
    
  - <span data-ttu-id="14664-114">[EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps)では、特定のメールボックスに RetentionHold の設定の状態を確認します。</span><span class="sxs-lookup"><span data-stu-id="14664-114">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/en-us/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="14664-115">特定のメールボックスでは、RetentionHold**を無効にするの**には、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="14664-115">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span> 
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="14664-116">ここで、管理フォルダー アシスタントを再実行します。</span><span class="sxs-lookup"><span data-stu-id="14664-116">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="14664-117">**注:** メールボックスが 10 MB より小さい場合は、管理フォルダー アシスタントはいない自動的にメールボックスの処理です。</span><span class="sxs-lookup"><span data-stu-id="14664-117">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span> 
  

