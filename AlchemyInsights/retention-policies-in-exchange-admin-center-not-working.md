---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: 3040365b9d686bcbcce60977ee9bdbbaffc70b24
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44502612"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="4b3a7-102">Exchange 管理センターでのアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="4b3a7-102">Retention Policies in Exchange Admin Center</span></span>

 <span data-ttu-id="4b3a7-103">**問題:** Exchange 管理センターで新規作成または更新したアイテム保持ポリシーがメールボックスに適用されないか、アイテムがアーカイブ メールボックスに移動または削除されません。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-103">**Issue:** Newly created or updated retention policies in the Exchange Admin Center are not applying to mailboxes or items are not moved to the archive mailbox or deleted.</span></span> 
  
 <span data-ttu-id="4b3a7-104">**原因:**</span><span class="sxs-lookup"><span data-stu-id="4b3a7-104">**Root Causes:**</span></span>
  
- <span data-ttu-id="4b3a7-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-105">This may be because the **Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="4b3a7-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-106">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span> <span data-ttu-id="4b3a7-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-107">If you change a retention tag or apply a different retention policy to a mailbox, you can wait until the Managed Folder Assist processes the mailbox, or you can run the Start-ManagedFolderAssistant cmdlet to start the Managed Folder Assistant to process a specific mailbox.</span></span> <span data-ttu-id="4b3a7-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-108">Running this cmdlet is useful for testing or troubleshooting a retention policy or retention tag settings.</span></span> <span data-ttu-id="4b3a7-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span><span class="sxs-lookup"><span data-stu-id="4b3a7-109">For more information, visit [Run the Managed Folder Assistant](https://msdn.microsoft.com/library/gg271153%28v=exchsrvcs.149%29.aspx#managedfolderassist).</span></span>
    
  - <span data-ttu-id="4b3a7-110">**解決方法:** 特定のメールボックスに対して管理フォルダー用アシスタントを開始するには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-110">**Solution:** Run the following command to start the Managed Folder Assistant for a specific mailbox:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

- <span data-ttu-id="4b3a7-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-111">This may also be occur if **RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="4b3a7-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span><span class="sxs-lookup"><span data-stu-id="4b3a7-112">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span> <span data-ttu-id="4b3a7-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="4b3a7-113">For more informaton on the RetentionHold setting see: [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
    
    <span data-ttu-id="4b3a7-114">**解決方法:**</span><span class="sxs-lookup"><span data-stu-id="4b3a7-114">**Solution:**</span></span>
    
  - <span data-ttu-id="4b3a7-115">[EXO Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps) を使用して、特定のメールボックスの保持ホールドの設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-115">Check the status of the RetentionHold setting on the specific mailbox in [EXO powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell?view=exchange-ps):</span></span>
    
  ```
  Get-Mailbox -Identity <name of the mailbox> |fl *retentionHold*
  ```

  - <span data-ttu-id="4b3a7-116">特定のメールボックスの保持ホールドを**無効**にするには、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-116">Run the following command to **disable** RetentionHold on a specific mailbox:</span></span>
    
  ```
  Set-Mailbox -RetentionHoldEnabled $false
  ```

  - <span data-ttu-id="4b3a7-117">次に、管理フォルダー用アシスタントを再実行します。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-117">Now, re-run the Managed folder Assistant:</span></span>
    
  ```
  Start-ManagedFolderAssistant -Identity <name of the mailbox>
  ```

 <span data-ttu-id="4b3a7-118">**注:** メールボックス サイズが 10 MB 未満の場合、管理フォルダー用アシスタントによってメールボックスは自動処理されません。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-118">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="4b3a7-119">Exchange 管理センターのアイテム保持ポリシーの詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4b3a7-119">For more info on retention policies in the Exchange Admin Center, see:</span></span>
- [<span data-ttu-id="4b3a7-120">保持タグおよびアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="4b3a7-120">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)
- [<span data-ttu-id="4b3a7-121">メールボックスにアイテム保持ポリシーを適用する</span><span class="sxs-lookup"><span data-stu-id="4b3a7-121">Apply a retention policy to mailboxes</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)
- [<span data-ttu-id="4b3a7-122">アイテム保持タグの追加または削除</span><span class="sxs-lookup"><span data-stu-id="4b3a7-122">Add or remove retention tags</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)
- [<span data-ttu-id="4b3a7-123">メールボックスに適用されている保留の種類を特定する方法</span><span class="sxs-lookup"><span data-stu-id="4b3a7-123">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
