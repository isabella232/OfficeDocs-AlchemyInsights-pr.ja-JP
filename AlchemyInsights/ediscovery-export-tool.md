---
title: 電子情報開示のエクスポート ツール
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "263"
- "928"
- "1100001"
- "3100022"
ms.assetid: b16d310d-1134-4959-be68-d1c0ad463930
ms.openlocfilehash: 67e59182a5053111a08f5fb2be814931a1aa815d
ms.sourcegitcommit: fbe6925797cab0b38172386f1b059dc122e452a4
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/25/2020
ms.locfileid: "48277951"
---
# <a name="cant-install-or-run-the-ediscovery-export-tool"></a><span data-ttu-id="c0254-102">電子情報開示のエクスポート ツールをインストールまたは実行できません。</span><span class="sxs-lookup"><span data-stu-id="c0254-102">Can't install or run the eDiscovery Export Tool?</span></span>

<span data-ttu-id="c0254-103">検索結果をダウンロードするために電子情報開示のエクスポート ツールをインストールしたり実行したりできない場合は、次のことをご確認ください。</span><span class="sxs-lookup"><span data-stu-id="c0254-103">If you can't install or run the eDiscovery Export Tool to download search results, check the following things:</span></span>
  
- <span data-ttu-id="c0254-104">使用するコンピューターは、次の前提条件を満たしている必要があります:</span><span class="sxs-lookup"><span data-stu-id="c0254-104">The computer you're using meets these pre-requisites:</span></span>

  - <span data-ttu-id="c0254-105">32 ビットおよび 64 ビット バージョンの Windows 7 およびそれ以降のバージョン</span><span class="sxs-lookup"><span data-stu-id="c0254-105">32- or 64-bit versions of Windows 7 and later versions</span></span>

  - <span data-ttu-id="c0254-106">Microsoft .NET Framework 4.7</span><span class="sxs-lookup"><span data-stu-id="c0254-106">Microsoft .NET Framework 4.7</span></span>

  - <span data-ttu-id="c0254-107">サポートされているブラウザー:</span><span class="sxs-lookup"><span data-stu-id="c0254-107">A supported browser:</span></span>

  - <span data-ttu-id="c0254-108">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c0254-108">Microsoft Edge</span></span>

    <span data-ttu-id="c0254-109">または</span><span class="sxs-lookup"><span data-stu-id="c0254-109">Or</span></span>

  - <span data-ttu-id="c0254-110">Internet Explorer 10 以降のバージョン</span><span class="sxs-lookup"><span data-stu-id="c0254-110">Internet Explorer 10 and later versions</span></span>

    <span data-ttu-id="c0254-111">Google Chrome や Mozilla Firefox など、他のブラウザーはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0254-111">Other browsers, such as Google Chrome and Mozilla Firefox aren't supported.</span></span>

- <span data-ttu-id="c0254-112">組織が Azure のエンドポイント (**\*.blob.core.windows.net**) に接続できます (ワイルドカードはエクスポート ジョブの一意の識別子を表します)。</span><span class="sxs-lookup"><span data-stu-id="c0254-112">Your organization can connect to the endpoint in Azure, which is **\*.blob.core.windows.net** (the wildcard represents a unique identifier for your export job).</span></span>

- <span data-ttu-id="c0254-p101">Microsoft 365 セキュリティ&amp;コンプライアンス センターで、ユーザーにエクスポートの役割が割り当てられています。既定では、この役割は電子情報開示管理者の役割グループにのみ割り当てられています。「[電子情報開示のアクセス許可を割り当てる](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0254-p101">You're assigned the Export role in the Microsoft 365 Security &amp; Compliance Center. By default, this role is only assigned to the eDiscovery Manager role group. See [Assign eDiscovery permissions](https://docs.microsoft.com/microsoft-365/compliance/assign-ediscovery-permissions).</span></span>

<span data-ttu-id="c0254-116">詳細については、「[コンテンツ検索の結果をエクスポートする](https://docs.microsoft.com/microsoft-365/compliance/export-search-results)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0254-116">For more information, see [Export Content Search results](https://docs.microsoft.com/microsoft-365/compliance/export-search-results).</span></span>

<span data-ttu-id="c0254-117">10万を超えるメールボックスをエクスポートする場合は、次の Powershell を使用してエクスポート結果をダウンロードする必要があります。  [10 万を超えるメールボックスから結果をエクスポート](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes)します。</span><span class="sxs-lookup"><span data-stu-id="c0254-117">If you are exporting more than 100K mailboxes, you will need to use the following Powershell to download the Export results:  [Exporting results from more than 100K mailboxes](https://docs.microsoft.com/microsoft-365/compliance/export-search-results?view=o365-worldwide%23exporting-results-from-more-than-100000-mailboxes).</span></span>