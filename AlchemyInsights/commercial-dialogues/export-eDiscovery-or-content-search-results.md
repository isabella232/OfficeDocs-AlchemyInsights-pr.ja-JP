---
title: 電子情報開示/コンテンツ検索結果をエクスポートする
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484152"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="2be55-102">電子情報開示/コンテンツ検索結果をエクスポートする</span><span class="sxs-lookup"><span data-stu-id="2be55-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="2be55-103">検索結果を PST ファイル (電子メールから) またはネイティブ Office ドキュメント (SharePoint および OneDrive for Business サイトから) にエクスポートする必要がある場合があります。</span><span class="sxs-lookup"><span data-stu-id="2be55-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="2be55-104">次の手順を実行してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-104">If so, do the following:</span></span>

- <span data-ttu-id="2be55-105">アカウントにエクスポートするための適切な権限が割り当てられていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="2be55-106">詳細については、「[電子情報開示権限のアクセス許可を割り当てる](https://go.microsoft.com/fwlink/?linkid=2102406)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="2be55-107">コンピュータがすべての[前提条件](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin)を満たしていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="2be55-108">Chrome など、すべてのブラウザがサポートされているわけではありません。</span><span class="sxs-lookup"><span data-stu-id="2be55-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="2be55-109">コンテンツ検索レポートをエクスポートするには: a.</span><span class="sxs-lookup"><span data-stu-id="2be55-109">To export from a Content Search: a.</span></span> <span data-ttu-id="2be55-110">[[セキュリティ/コンプライアンス センター]](https://protection.office.com/contentsearch)に移動し、**[検索]** をクリックして、**[コンテンツ検索]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="2be55-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="2be55-111">**[コンテンツ検索]** ページで、保存した検索を選択します。</span><span class="sxs-lookup"><span data-stu-id="2be55-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="2be55-112">b.</span><span class="sxs-lookup"><span data-stu-id="2be55-112">b.</span></span> <span data-ttu-id="2be55-113">詳細ウィンドウの **[結果をコンピューターにエクスポートする]** で、**[エクスポートの開始]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="2be55-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="2be55-114">10 万を超えるメール ボックスをエクスポートする場合は、PowerShell を使用してエクスポート結果をダウンロードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2be55-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="2be55-115">詳細については、「[100,000 を超えるメールボックスからの結果のエクスポート](https://go.microsoft.com/fwlink/?linkid=2143861)」参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="2be55-116">詳細については、「[コンテンツ検索の結果をエクスポートする](https://go.microsoft.com/fwlink/?linkid=2102118)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2be55-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>