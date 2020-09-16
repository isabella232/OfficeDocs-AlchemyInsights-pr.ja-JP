---
title: Teams のプライベート チャネルを削除する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 56021a335c64810700913cf08519b95f24a7a17d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47730920"
---
# <a name="delete-a-teams-private-channel"></a><span data-ttu-id="a73f0-102">Teams のプライベート チャネルを削除する</span><span class="sxs-lookup"><span data-stu-id="a73f0-102">Delete a Teams private channel</span></span>

<span data-ttu-id="a73f0-103">Microsoft は、もし基になる SharePoint サイトに対して SharePoint アイテム保持ポリシーが有効だと、Teams のプライベート チャネルが削除されるという問題を認識しています。</span><span class="sxs-lookup"><span data-stu-id="a73f0-103">Microsoft is aware of an issue deleting a Teams private channel if you have SharePoint Retention Policies enabled for the underlying SharePoint site.</span></span> <span data-ttu-id="a73f0-104">Microsoft は解決に取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="a73f0-104">Microsoft is working on a fix.</span></span> <span data-ttu-id="a73f0-105">それまでは、次の回避策を使用してプライベート チャネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a73f0-105">In the meantime, you can use the following workarounds to delete the private channel.</span></span>

<span data-ttu-id="a73f0-106">**Sharepoint アイテム保持ポリシーから Team /サイトコレクションを除外します。**</span><span class="sxs-lookup"><span data-stu-id="a73f0-106">**Exclude the Team/site collection from the Sharepoint retention policy.**</span></span>

1. <span data-ttu-id="a73f0-107">Office 365 管理ポータルに移動し、左側のナビゲーション ウィンドウで [**すべて表示**] を選択します。</span><span class="sxs-lookup"><span data-stu-id="a73f0-107">Go to the Office 365 admin portal, and select **Show all** in the left navigation pane.</span></span>
2. <span data-ttu-id="a73f0-108">[**管理センター**] の下にある [**セキュリティ/コンプライアンス** > **データ損失防止** > **ポリシー**] に移動します。</span><span class="sxs-lookup"><span data-stu-id="a73f0-108">Under **Admin centers**, go to **Security & Compliance** > **Data Loss Prevention** > **Policy**.</span></span>
3. <span data-ttu-id="a73f0-109">Sharepoint サイトに適用されるポリシーすべてを特定し、プライベート チャネルを含む Team の Sharepoint サイトがアイテム保持ポリシーに含まれないように、そのポリシーを変更します。</span><span class="sxs-lookup"><span data-stu-id="a73f0-109">Identify any policy that applies to Sharepoint sites, and modify the policy so the Sharepoint site for the Team containing the private channel is NOT included under the retention policy.</span></span>
4. <span data-ttu-id="a73f0-110">ポリシーを保存します。</span><span class="sxs-lookup"><span data-stu-id="a73f0-110">Save the policy.</span></span>
    <span data-ttu-id="a73f0-111">ポリシー設定が有効になるまで最大 24 時間かかる場合があります。</span><span class="sxs-lookup"><span data-stu-id="a73f0-111">It can take up to 24 hours for policy settings to take effect.</span></span>
    <span data-ttu-id="a73f0-112">サイトを除外したら、プライベート チャネルを削除できます。</span><span class="sxs-lookup"><span data-stu-id="a73f0-112">After the site has been excluded, you can delete the private channel.</span></span>  
    
<span data-ttu-id="a73f0-113">お客様の Android デバイスで Microsoft Teams を使用すると、プライベート チャネルを削除できる ***可能性*** があります。</span><span class="sxs-lookup"><span data-stu-id="a73f0-113">You  ***might*** be able to delete the private channel by using Microsoft Teams on your Android device.</span></span> 

<span data-ttu-id="a73f0-114">関連する SharePoint の詳細については、[SharePoint Online または OneDrive for Business でアイテムを削除できない](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a73f0-114">For related SharePoint information, see [Unable to delete items in SharePoint Online or OneDrive for Business](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).</span></span>