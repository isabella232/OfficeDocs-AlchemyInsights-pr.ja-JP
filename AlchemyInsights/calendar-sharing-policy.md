---
title: 618 予定表の共有ポリシー
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373004"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="a6213-102">予定表を共有する場合のポリシー エラー</span><span class="sxs-lookup"><span data-stu-id="a6213-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="a6213-103">状況に応じて、次のいずれかを実行します。</span><span class="sxs-lookup"><span data-stu-id="a6213-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="a6213-104">リモート PowerShell を使用して Exchange Online に接続します。</span><span class="sxs-lookup"><span data-stu-id="a6213-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="a6213-105">詳細については、「[リモート PowerShell による Exchange への接続](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6213-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="a6213-106">オンプレミスのサーバーで Exchange 管理シェルを開きます。</span><span class="sxs-lookup"><span data-stu-id="a6213-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="a6213-107">ユーザーに割り当てられている共有ポリシーを決定します。</span><span class="sxs-lookup"><span data-stu-id="a6213-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="a6213-108">これを行うには、次のコマンドを実行して、返されたポリシーを確認します。</span><span class="sxs-lookup"><span data-stu-id="a6213-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="a6213-109">ユーザーの共有ポリシーを更新します。</span><span class="sxs-lookup"><span data-stu-id="a6213-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="a6213-110">これを行うには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="a6213-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="a6213-111">Exchange 管理センターを開きます。</span><span class="sxs-lookup"><span data-stu-id="a6213-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="a6213-112">[**組織**] をクリックし、[**個別共有**] でユーザーに割り当てられているポリシーをダブルクリックします。</span><span class="sxs-lookup"><span data-stu-id="a6213-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="a6213-113">これは、手順 2 で返されたポリシーです。</span><span class="sxs-lookup"><span data-stu-id="a6213-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="a6213-114">[共有ルール] ページの [**共有する情報を指定します**] で、許可する予定表の共有レベルを選択します。[**保存**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="a6213-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="a6213-115">予定表を共有しようとしているときに、詳細情報については、「[このレベルのアクセス権限を 1 人以上の受信者に付与することは、ポリシーで許可されていません](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue)」エラーを参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6213-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
