---
title: ルート サイトとしてのモダン サイト
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid:
- "9000153"
- "1692"
ms.openlocfilehash: 6f55f1c63551027cc5522d296cb3f3f342356d95
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/18/2019
ms.locfileid: "36576690"
---
# <a name="modernize-your-classic-sharepoint-site"></a><span data-ttu-id="3930c-102">従来の SharePoint サイトをモダン化する</span><span class="sxs-lookup"><span data-stu-id="3930c-102">Modernize your classic SharePoint sites</span></span>

<span data-ttu-id="3930c-103">モダン ユーザー インターフェイスに切り替える場合、以下の点に注意してください:</span><span class="sxs-lookup"><span data-stu-id="3930c-103">To make the switch to a modern user interface, you need to focus on the following:</span></span>

- <span data-ttu-id="3930c-104">**リストとライブラリ**がモダン ユーザー インターフェイス (モダン リスト エクスペリエンスやモダン ライブラリ エクスペリエンスとも呼ばれる) を使用するようにする。</span><span class="sxs-lookup"><span data-stu-id="3930c-104">Transitioning your **lists and libraries** to use the modern user interface (also referred to as the modern list and library experience)</span></span>
- <span data-ttu-id="3930c-105">**サイト ページ**を従来型の Wiki ページや Web パーツ ページからクライアント側モダン ページに変換する。</span><span class="sxs-lookup"><span data-stu-id="3930c-105">Transforming your **site pages** from classic wiki and web part pages into modern client-side pages</span></span>
- <span data-ttu-id="3930c-106">**モダン サイト** (チーム サイトまたはコミュニケーション サイト) を作成する。</span><span class="sxs-lookup"><span data-stu-id="3930c-106">Creating **modern sites** (Team site or Communication Site).</span></span>

<span data-ttu-id="3930c-107">次の方法で、エクスペリエンスをモダン化します。</span><span class="sxs-lookup"><span data-stu-id="3930c-107">Modernize your user experience by:</span></span>
- <span data-ttu-id="3930c-108">カスタマイズを置き換えるか、互換性のない列を使用するビューから削除するか、(最終手段として) データをモダン ユーザー インターフェイスと互換性のあるリスト型に移動することにより、[リストとライブラリがモダン ユーザー インターフェイスで表示](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries)されるようにします。</span><span class="sxs-lookup"><span data-stu-id="3930c-108">[Enabling lists and libraries to show in the modern user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) by replacing customizations, removing incompatible columns from the used views, or (as a last resort) moving data into a modern user interface-compatible list type.</span></span>
- <span data-ttu-id="3930c-109">[サイトを Office 365 グループに接続](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group)します。その結果、サイトにモダン ホーム ページが作成され、サイトでメールボックスや Microsoft Planner などが使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="3930c-109">[Connecting your site to an Office 365 group](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), which gives your site a modern home page and enables your site to use, for example, a mailbox or Microsoft Planner, which then enables you to use a modern version of a calendar and task list.</span></span> <span data-ttu-id="3930c-110">これにより、ユーザーはモダン バージョンのカレンダーやタスク リストを使用できるようになります。</span><span class="sxs-lookup"><span data-stu-id="3930c-110">This enables you to use a modern version of a calendar and task list.</span></span>
- <span data-ttu-id="3930c-111">[モダン ページの作成](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec)は、画像、Excel、Word、PowerPoint ドキュメント、ビデオ、その他を使用してアイデアを共有する優れた方法です。</span><span class="sxs-lookup"><span data-stu-id="3930c-111">[Creating modern pages](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), is a great way to share ideas using images, Excel, Word and PowerPoint documents, video, and more.</span></span>
- <span data-ttu-id="3930c-112">[クライアント側モダン ページを作成](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages)し、従来型の主要な Wiki ページや Web パーツ ページと似たものになるように構成します。</span><span class="sxs-lookup"><span data-stu-id="3930c-112">[Creating modern client-side pages](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) and configuring these to be "similar" to your key classic wiki and web part pages.</span></span> <span data-ttu-id="3930c-113">プログラムによるページ変換は、サイトの主要なページに対して実行するようにお勧めします。これは、すべてのページを変換することは、リソースの消費になるだけでなく、多くの場合必要ないためです。</span><span class="sxs-lookup"><span data-stu-id="3930c-113">Programmatic page transformation should be done for the key pages of your sites; transforming all pages is resource-intensive and often not needed.</span></span> <span data-ttu-id="3930c-114">このトリアージを支援するため、SharePoint モダン化スキャナーを使用すると、現在の Wiki ページや Web パーツ ページの閲覧状況に関する情報が得られます。</span><span class="sxs-lookup"><span data-stu-id="3930c-114">To assist in this triage, the SharePoint Modernization scanner can give you usage information about the current wiki and web part pages.</span></span>
- <span data-ttu-id="3930c-115">[モダン サイトの作成](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d)。</span><span class="sxs-lookup"><span data-stu-id="3930c-115">Creating modern sites</span></span> <span data-ttu-id="3930c-116">チーム サイトまたはコミュニケーション サイトを作成する必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="3930c-116">Should I create a team site or a communication site?</span></span>

<span data-ttu-id="3930c-117">追加情報:</span><span class="sxs-lookup"><span data-stu-id="3930c-117">Additional info</span></span> 
- <span data-ttu-id="3930c-118">従来の SharePoint サイトをモダン エクスペリエンスにモダン化する手順の概要については、「[従来の SharePoint サイトをモダン化する](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3930c-118">For a step-by-step overview of modernizing your classic SharePoint Sites to the modern experience, see [Modernize your classic SharePoint Sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span></span>
- <span data-ttu-id="3930c-119">「[モダン エクスペリエンス](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience)」のガイドを参照してください。</span><span class="sxs-lookup"><span data-stu-id="3930c-119">See a guide to [Modern Experience](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span></span>
- <span data-ttu-id="3930c-120">「[従来の SharePoint および最新のエクスペリエンス](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3930c-120">See [SharePoint Classic and Modern experiences](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span></span> 




