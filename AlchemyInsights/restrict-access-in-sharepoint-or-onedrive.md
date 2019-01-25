---
title: SharePoint または OneDrive でのアクセスを制限します。
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29476953"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="cdec8-102">SharePoint または OneDrive でのアクセスを制限します。</span><span class="sxs-lookup"><span data-stu-id="cdec8-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="cdec8-p101">SharePoint および OneDrive は、アクセスを制限するファイル、フォルダー、およびリストなどの項目をグループまたは個人のアクセスが必要なだけにアクセスを付与することによって。既定では、SharePoint のアクセス許可は、階層の上位にあるほどから継承されます。ファイルは、サイトからアクセス許可を継承すると、ライブラリのアクセス許可を継承すると、フォルダーからアクセス許可を継承します。</span><span class="sxs-lookup"><span data-stu-id="cdec8-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="cdec8-p102">高いレベルで共有することができます (次のようにサイト全体を共有することによって)、サイトのすべてのアイテムを共有したくない場合、継承を停止します。ただし、お勧めしませんこのアクセス許可の維持より複雑でわかりにくく、将来的にするためです。代わりに行うことは可能です。</span><span class="sxs-lookup"><span data-stu-id="cdec8-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="cdec8-109">場合は、たとえば、フォルダー内に 1 つのファイル以外のすべての内容を共有する、共有されていない別の場所にそのファイルを移動します。</span><span class="sxs-lookup"><span data-stu-id="cdec8-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="cdec8-110">フォルダーに 2 つのサブフォルダーがある場合は A と B のグループで 1 つのサブフォルダーを共有のみグループ A、2 つ目のサブフォルダーにアクセスを許可、グループ A と親フォルダーを共有し、グループ B の最初のサブフォルダーを追加します。</span><span class="sxs-lookup"><span data-stu-id="cdec8-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="cdec8-111">ファイルまたはフォルダーの共有を停止します。</span><span class="sxs-lookup"><span data-stu-id="cdec8-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

