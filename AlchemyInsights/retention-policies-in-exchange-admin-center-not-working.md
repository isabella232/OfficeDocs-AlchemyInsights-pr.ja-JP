---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 5d7b62546397c13b37540e8797b31123b2880280
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551348"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a88bf-102">Exchange 管理センターでのアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="a88bf-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="a88bf-103">**問題:** Exchange 管理センターで新規作成または更新したアイテム保持ポリシーがメールボックスに適用されないか、アイテムがアーカイブ メールボックスに移動または削除されません。</span><span class="sxs-lookup"><span data-stu-id="a88bf-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="a88bf-104">**原因:**</span><span class="sxs-lookup"><span data-stu-id="a88bf-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="a88bf-p101">これは、**管理フォルダー用アシスタント**が、ユーザーのメールボックスを処理していないことが原因である可能性があります。管理フォルダー用アシスタントは、クラウド ベースの組織のすべてのメールボックスの処理を 7 日間に 1 回試行します。ユーザーが保持タグを変更した場合やメールボックスに別のアイテム保持ポリシーを適用した場合は、管理フォルダー アシスタントによってメールボックスが処理されるまで待つか、Start-ManagedFolderAssistant コマンドレットを実行して、管理フォルダー用アシスタントによって特定のメールボックスの処理が開始されるようにします。このコマンドレットの実行は、アイテム保持ポリシーまたは保持タグの設定をテストまたはトラブルシューティングするのに便利です。詳細については、[管理フォルダー用アシスタントの実行](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a88bf-p101">This may be because the **Managed Folder Assistant** has not processed the user's mailbox. The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days. If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox. Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings. For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="a88bf-110">**解決方法:** 特定のメールボックスに対して管理フォルダー用アシスタントを開始するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="a88bf-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="a88bf-p102">これは、メールボックスで**保持ホールド**が**有効**になっている場合にも発生する可能性があります。メールボックスが保持ホールドになっている場合、その期間、そのメールボックスに対してアイテム保持ポリシーは処理されません。保持ホールドの設定の詳細については、[メールボックスの保持ホールド](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a88bf-p102">This may also be occur if **RetentionHold** has been **enabled** on the mailbox. If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time. For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="a88bf-114">**解決方法:**</span><span class="sxs-lookup"><span data-stu-id="a88bf-114">**Solution:**</span></span>
    
  - <span data-ttu-id="a88bf-115">[EXO Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) を使用して、特定のメールボックスの保持ホールドの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="a88bf-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="a88bf-116">特定のメールボックスの保持ホールドを**無効**にするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="a88bf-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="a88bf-117">次に、管理フォルダー用アシスタントを再実行します。</span><span class="sxs-lookup"><span data-stu-id="a88bf-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="a88bf-118">**注:** メールボックス サイズが 10 MB 未満の場合、管理フォルダー用アシスタントによってメールボックスは自動処理されません。</span><span class="sxs-lookup"><span data-stu-id="a88bf-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a88bf-119">Exchange 管理センターのアイテム保持ポリシーの詳細については、次の情報を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a88bf-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="a88bf-120">保持タグおよびアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="a88bf-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="a88bf-121">メールボックスにアイテム保持ポリシーを適用する</span><span class="sxs-lookup"><span data-stu-id="a88bf-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="a88bf-122">アイテム保持タグの追加または削除</span><span class="sxs-lookup"><span data-stu-id="a88bf-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="a88bf-123">メールボックスにかけられた保留の種類を識別する方法</span><span class="sxs-lookup"><span data-stu-id="a88bf-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/office365/securitycompliance/identify-a-hold-on-an-exchange-online-mailbox)
