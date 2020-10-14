---
title: SharePoint または OneDrive でアクセスを制限する
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720687"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="388eb-102">SharePoint または OneDrive でアクセスを制限する</span><span class="sxs-lookup"><span data-stu-id="388eb-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="388eb-p101">SharePoint と OneDrive では、アクセスを許可する必要のあるグループまたは個人にのみアクセス権を付与することにより、ファイル、フォルダー、リストなどのアイテムへのアクセスを制限します。既定では、SharePoint でのアクセス許可は階層内の上位から継承されます。そのため、ファイルのアクセス許可はフォルダーから継承され、フォルダーのアクセス許可はライブラリから継承され、ライブラリのアクセス許可はサイトから継承されます。</span><span class="sxs-lookup"><span data-stu-id="388eb-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="388eb-p102">(サイト全体を共有するなどして) より高いレベルで共有することができますが、サイト上のすべてのアイテムを共有したいわけではない場合は継承設定を解除することもできます。ただし、これは推奨しません。アクセス許可の維持がより複雑になり、将来的に混乱を招くことになるためです。継承設定の解除に代わる可能な方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="388eb-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="388eb-109">たとえば、フォルダー内で 1 つのファイルを除くすべてのコンテンツを共有する場合は、その 1 つのファイルを共有されていない新しい場所に移動します。</span><span class="sxs-lookup"><span data-stu-id="388eb-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="388eb-110">フォルダーに 2 つのサブフォルダーがある場合、1 つ目のサブフォルダーをグループ A およびグループ B と共有し、かつグループ A のみに 2 つ目のサブフォルダーへのアクセスを許可するには、親フォルダーをグループ A と共有し、1 つ目のサブフォルダーにグループ B を追加します。</span><span class="sxs-lookup"><span data-stu-id="388eb-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="388eb-111">ファイルまたはフォルダーの共有を停止する</span><span class="sxs-lookup"><span data-stu-id="388eb-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

