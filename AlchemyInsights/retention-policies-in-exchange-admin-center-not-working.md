---
title: Exchange 管理センターでアイテム保持ポリシーが動作しない
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
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952233"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="a6827-102">Exchange 管理センターでのアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="a6827-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="a6827-103">下記の設定の自動チェックを実行する場合は、このページの上部にある [戻る <--] ボタンを選択し、メールをアーカイブメールボックスに移動できないユーザーのメールアドレスを入力します。</span><span class="sxs-lookup"><span data-stu-id="a6827-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="a6827-104">Exchange 管理センターのアイテム保持ポリシーがメールボックスに適用されない、またはアイテムがアーカイブ メールボックスに移動しないという問題がある場合は、以下を確認してください。</span><span class="sxs-lookup"><span data-stu-id="a6827-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="a6827-105">**根本原因:**</span><span class="sxs-lookup"><span data-stu-id="a6827-105">**Root Causes:**</span></span>

- <span data-ttu-id="a6827-106">**管理フォルダー用アシスタント** はユーザーのメールボックスを処理していません。</span><span class="sxs-lookup"><span data-stu-id="a6827-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="a6827-107">管理フォルダー用アシスタントは、7 日に一度クラウドベース組織のすべてのメールボックスを処理しようとします。</span><span class="sxs-lookup"><span data-stu-id="a6827-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="a6827-108">**解決策:** 管理フォルダー用アシスタントを実行します。</span><span class="sxs-lookup"><span data-stu-id="a6827-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="a6827-109">メールボックスで **RetentionHold** が **有効** になっています。</span><span class="sxs-lookup"><span data-stu-id="a6827-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="a6827-110">メールボックスが RetentionHold に配置されている場合、その間、メールボックスのアイテム保持ポリシーは処理されません。</span><span class="sxs-lookup"><span data-stu-id="a6827-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="a6827-111">**解決策:** 保持ホールド設定の状態を確認し、必要に応じて更新します。</span><span class="sxs-lookup"><span data-stu-id="a6827-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="a6827-112">詳細については、「[メールボックスのアイテム保持ホールド](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6827-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="a6827-113">**注:** メールボックス サイズが 10 MB 未満の場合、管理フォルダー用アシスタントによってメールボックスは自動処理されません。</span><span class="sxs-lookup"><span data-stu-id="a6827-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="a6827-114">Exchange 管理センターのアイテム保持ポリシーの詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6827-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="a6827-115">保持タグおよびアイテム保持ポリシー</span><span class="sxs-lookup"><span data-stu-id="a6827-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="a6827-116">[メールボックスにアイテム保持ポリシーを適用する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy)か、[アイテム保持タグを追加または削除する](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="a6827-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="a6827-117">メールボックスに適用されている保留の種類を特定する方法</span><span class="sxs-lookup"><span data-stu-id="a6827-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
