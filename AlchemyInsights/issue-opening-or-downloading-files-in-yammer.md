---
title: Yammer でファイルを開いたり、ダウンロードしたりする際の問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695654"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="cb883-102">Yammer でファイルを開いたり、ダウンロードしたりする際の問題</span><span class="sxs-lookup"><span data-stu-id="cb883-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="cb883-103">従来の Yammer は、メッセージおよびグループへのファイルのアップロードについて、複数のオプションをサポートしています。</span><span class="sxs-lookup"><span data-stu-id="cb883-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="cb883-104">ネットワーク構成によっては、ファイルは、既定で SharePoint のストレージに保存されます。</span><span class="sxs-lookup"><span data-stu-id="cb883-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="cb883-105">新しい Yammer のファイルピッカーは、従来の Yammer で使用可能なすべてのオプションをまだサポートしていません。</span><span class="sxs-lookup"><span data-stu-id="cb883-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="cb883-106">今後の更新で、追加の機能が追加されます。</span><span class="sxs-lookup"><span data-stu-id="cb883-106">A future update will add additional features.</span></span> <span data-ttu-id="cb883-107">詳しくは、[「Yammer の会話の投稿にファイルまたは画像を添付する」](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="cb883-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="cb883-108">**ファイルを開くことができない、またはダウンロードすることができない**</span><span class="sxs-lookup"><span data-stu-id="cb883-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="cb883-109">ファイルを Yammer にアップロードしたり、SharePoint Online のファイルにリンクしたりすることもできます。</span><span class="sxs-lookup"><span data-stu-id="cb883-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="cb883-110">トラブルシューティングを行うには、まずファイルの場所を特定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cb883-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="cb883-111">ファイルが Yammer にアップロードされている場合、ファイルの URL は \* yammer.com です。</span><span class="sxs-lookup"><span data-stu-id="cb883-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="cb883-112">必要な URLと IP アドレスがブロック解除されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="cb883-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="cb883-113">詳細については、ブログの投稿[Yammer にハードコードされた IP アドレスを使用することはお勧めできません](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb883-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="cb883-114">グローバル管理者でもあるユーザーがファイルをダウンロードできるかどうかを確認します。</span><span class="sxs-lookup"><span data-stu-id="cb883-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="cb883-115">ファイルが個人用の場合、プライベートコンテンツモードを使用する必要がある可能性があります。</span><span class="sxs-lookup"><span data-stu-id="cb883-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="cb883-116">詳細については、[「Yammerでプライベートコンテンツ を監視する」](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb883-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="cb883-117">**Yammer ネットワークのゲストと SharePoint Online のファイル**</span><span class="sxs-lookup"><span data-stu-id="cb883-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="cb883-118">[Yammer のネットワークゲスト](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests)は、Azure AD B2B を使わず、Yammer サービスの内部にあるため、SharePoint に保存されている Yammer ファイルにアクセスできません。</span><span class="sxs-lookup"><span data-stu-id="cb883-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="cb883-119">ID を使用して、SharePoint Online のドキュメントライブラリにアクセスできる外部 AAD B2B ユーザーを作成します。</span><span class="sxs-lookup"><span data-stu-id="cb883-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="cb883-120">Yammer での Azure AD B2B ゲストサポートの詳細については、[「Yammerプレビューで企業間 (B2B)での ゲストサポート- お客様のご利用規約と よくあるご質問」](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb883-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>