---
title: SharePoint ドキュメント ライブラリでアイテムをコピーまたは移動する
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 5/24/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "454"
- "5300013"
ms.assetid: 592f502a-493f-4bf4-adc3-5bc8aea87bb5
ms.openlocfilehash: 6e14260d3670eb15f73e92dc5b0c86e0e842974a
ms.sourcegitcommit: efdde3c24a0c1adfb8b6f5f59dcae435fb5c53a8
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/19/2019
ms.locfileid: "38711761"
---
# <a name="copy-or-move-items-in-a-sharepoint-document-library"></a><span data-ttu-id="b9371-102">SharePoint ドキュメント ライブラリでアイテムをコピーまたは移動する</span><span class="sxs-lookup"><span data-stu-id="b9371-102">Copy or move items in a SharePoint document library</span></span>

<span data-ttu-id="b9371-p101">ドキュメントライブラリ内の別の場所にファイル、フォルダー、およびリンクをコピーして移動することができます。サイト間でアイテムをコピーすることもできます。</span><span class="sxs-lookup"><span data-stu-id="b9371-p101">You can copy and move files, folders, and links to different locations within a document library. You can also copy items across sites.</span></span> 
  
1. <span data-ttu-id="b9371-105">ブラウザーで、移動するファイル、フォルダー、またはリンクを参照して、**[コピー先]** または **[移動先]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b9371-105">In a browser, browse to the files, folders, or links you want to move, and then click **Copy to** or **Move to**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b9371-106">SharePoint Online のクラシック環境を使用している場合、**[コピー先]** および **[移動先]** は使用できません。</span><span class="sxs-lookup"><span data-stu-id="b9371-106">**Copy to** and **Move to** aren't available if you're using the classic experience of SharePoint Online.</span></span>
  
2. <span data-ttu-id="b9371-107">**[移動先の選択]** で、アイテムをコピーまたは移動する場所を選択するか、**[サイトの参照]** をクリックしてサイトの全リストを表示します。</span><span class="sxs-lookup"><span data-stu-id="b9371-107">Under **Choose a destination**, select the location to which you want to copy or move the items or click **Browse sites** to see the full list of sites.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b9371-p102">アイテムをコピーするときに他のサイトが一覧表示されない場合は、サイト間でのコピーが構成されていません。この操作を有効にするには、SharePoint 管理センターの設定ページに移動し、**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b9371-p102">If you don't see other sites listed when you copy items, copying across sites hasn't been configured. To enable it, go to the settings page of the SharePoint admin center and click **OK**.</span></span>
  
    <span data-ttu-id="b9371-110">新しいフォルダーを作成する場合は、フォルダー階層内の場所を選択して **[新しいフォルダー]** をクリックします。次にフォルダー名を入力し、チェック マークをクリックして名前を保存します。</span><span class="sxs-lookup"><span data-stu-id="b9371-110">To create a new folder, select a location in the folder hierarchy, click **New folder**, enter a name for the folder, and click the check mark to save the name.</span></span>

3. <span data-ttu-id="b9371-111">**[ここにコピー]** または **[ここに移動]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="b9371-111">Click **Copy here** or **Move here**.</span></span>

    > [!NOTE]
    > <span data-ttu-id="b9371-p103">一度に最大 500 MB のファイルおよびフォルダーをコピーできます。> バージョン履歴を含むドキュメントをコピーすると、最新バージョンのみがコピーされます。ドキュメントを移動すると、その履歴も移動されます。</span><span class="sxs-lookup"><span data-stu-id="b9371-p103">You can copy up to 500 MB of files and folders at one time. >  When you copy documents that have version history, only the latest version is copied. When you move documents, their history is also moved.</span></span>
  
 <span data-ttu-id="b9371-115">ファイルが移動されると、移動先に完全に移動されるまでソースディレクトリに表示されたままになり、削除されます。</span><span class="sxs-lookup"><span data-stu-id="b9371-115">When a file is moving, it will still appear in the source directory until its fully moved to the destination, and then it will be deleted.</span></span> <span data-ttu-id="b9371-116">このファイルは、移動が完了した後にソースサイトのごみ箱に残り、ユーザーがごみ箱から回復しない限り、通常のリサイクルスケジュールに従います。</span><span class="sxs-lookup"><span data-stu-id="b9371-116">The file will remain in the source sites recycle bin after the move is complete and be subject to the normal recycle schedule unless a user recovers it from the recycle bin.</span></span>

<span data-ttu-id="b9371-117">詳細については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9371-117">For more information, see:</span></span>

 - <span data-ttu-id="b9371-118">[SharePoint でファイルを移動またはコピー](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc)する (Office サポート記事)</span><span class="sxs-lookup"><span data-stu-id="b9371-118">[Move or copy files in SharePoint](https://support.office.com/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc) (Office support article)</span></span>
 - <span data-ttu-id="b9371-119">[Office 365 の任意のフォルダーからファイルを移動](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973)する (Microsoft Tech Community ブログ記事)</span><span class="sxs-lookup"><span data-stu-id="b9371-119">[Move files from any folder in Office 365](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Now-move-files-anywhere-in-Office-365-SharePoint-and-OneDrive/ba-p/146973) (Microsoft Tech Community blog article)</span></span>  