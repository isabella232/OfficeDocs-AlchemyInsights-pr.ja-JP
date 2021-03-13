---
title: 組織内の電子メールメッセージの検索と削除
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000260"
- "7257"
ms.openlocfilehash: e935b10083459b81fc58e12bb59c9511defefa6d
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/11/2021
ms.locfileid: "50751372"
---
# <a name="search-for-and-delete-email-messages-in-your-organization"></a><span data-ttu-id="7117e-102">組織内の電子メールメッセージの検索と削除</span><span class="sxs-lookup"><span data-stu-id="7117e-102">Search for and delete email messages in your organization</span></span>

<span data-ttu-id="7117e-103">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="7117e-103">Follow these steps:</span></span>

1. <span data-ttu-id="7117e-104">グローバル管理者ではない場合、メッセージを検索するには、自分のアカウントを **電子情報開示マネージャー役割グループ** または **コンプライアンス検索管理の役割** に追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="7117e-104">If you're not a global admin, to search for messages your account must be added to the **eDiscovery Manager role group** or **Compliance Search management role**.</span></span> <span data-ttu-id="7117e-105">メッセージを削除するには、**組織管理の役割グループ** のメンバーであるか、**検索と消去の管理の役割** が割り当てられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7117e-105">To delete messages, you'll need to join the **Organization Management role group** or the **Search and Purge management role**.</span></span> <span data-ttu-id="7117e-106">これらの役割へのアクセス許可は、[セキュリティ/コンプライアンス センター](https://protection.office.com)で割り当てられます。</span><span class="sxs-lookup"><span data-stu-id="7117e-106">Permissions to these roles are assigned in the [Security & compliance center.](https://protection.office.com)</span></span>
2. <span data-ttu-id="7117e-107">[コンテンツ検索を作成し、](https://docs.microsoft.com/office365/securitycompliance/content-search) 削除するメッセージを見つけます。</span><span class="sxs-lookup"><span data-stu-id="7117e-107">[Create a content search](https://docs.microsoft.com/office365/securitycompliance/content-search) to find the message to delete.</span></span>
3. <span data-ttu-id="7117e-108">[セキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="7117e-108">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span> <span data-ttu-id="7117e-109">MFA をお使いの場合は、「[多要素認証を使用してセキュリティ/コンプライアンス センターの PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)」の手順を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7117e-109">If you're using MFA, see these instructions: [Connect to Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)</span></span>
4. <span data-ttu-id="7117e-110">メッセージを削除します。`New-ComplianceSearchAction` コマンドレットを実行してメッセージを削除します。</span><span class="sxs-lookup"><span data-stu-id="7117e-110">Delete the message: run the `New-ComplianceSearchAction` cmdlet to delete the message.</span></span> <span data-ttu-id="7117e-111">削除されたメッセージは、ユーザーの [回復可能なアイテム] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="7117e-111">Deleted messages are moved to a user's Recoverable Items folder.</span></span> <span data-ttu-id="7117e-112">コマンドの例については、「[手順 3: メッセージを削除する](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7117e-112">For an example command, see [Step 3: Delete the message.](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messages-in-your-organization)</span></span>
