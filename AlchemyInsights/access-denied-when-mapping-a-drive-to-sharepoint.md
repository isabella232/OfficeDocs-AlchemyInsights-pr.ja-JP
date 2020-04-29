---
title: ドライブを SharePoint にマップしようとするとアクセスが拒否される
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: b7da3918-969f-40bb-acb3-fbc762605504
ms.openlocfilehash: 23ee86df5404b6f20f3a4b605038b31b6f9fd731
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43687371"
---
# <a name="fix-problems-with-sharepoint-libraries-mapped-to-network-drives"></a><span data-ttu-id="311de-102">ネットワーク ドライブにマップされた SharePoint ライブラリに関する問題を修正します</span><span class="sxs-lookup"><span data-stu-id="311de-102">Fix problems with SharePoint libraries mapped to network drives</span></span>

<span data-ttu-id="311de-103">マップされたネットワーク ドライブを参照すると、次のいずれかのメッセージが表示されることがあります。</span><span class="sxs-lookup"><span data-stu-id="311de-103">When you browse to a mapped network drive, you may see one of the following messages:</span></span>
  
- <span data-ttu-id="311de-104">**\\パスにアクセスできません。このネットワーク リソースを使用するアクセス許可がない可能性があります。アクセス許可があるかどうかを確認するには、このサーバーの管理者に問い合わせてください。**</span><span class="sxs-lookup"><span data-stu-id="311de-104">**\\Path is not accessible. You might not have permission to use this network resource. Contact the administrator of this server to find out if you have access permissions.**</span></span>

- <span data-ttu-id="311de-105">**アクセスが拒否されました。この場所のファイルを開く前に、まず Web サイトを信頼済みサイトのリストに追加し、Web サイトを参照して、自動的にログインするオプションを選択してください。**</span><span class="sxs-lookup"><span data-stu-id="311de-105">**Access Denied. Before opening files in this location, you must first add the web site to your trusted site list, browse to the web site, and select the option to login automatically.**</span></span>

<span data-ttu-id="311de-106">[マップされたネットワーク ドライブのトラブルシューティングのヘルプを表示します](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives)。</span><span class="sxs-lookup"><span data-stu-id="311de-106">[Get help troubleshooting mapped network drives](https://docs.microsoft.com/sharepoint/support/administration/troubleshoot-mapped-network-drives).</span></span>
  
<span data-ttu-id="311de-p101">ライブラリをネットワーク ドライブとしてマップすることは一時的であり、Internet Explorer でのみサポートされています。その代わりに、[ファイル オンデマンド](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx)を含む[新しい OneDrive 同期クライアントを使用して SharePoint ファイルを同期](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx)します。OneDrive 内のすべてのファイルに、ローカル記憶域を使用することなくアクセスします。</span><span class="sxs-lookup"><span data-stu-id="311de-p101">Mapping a library as a network drive is temporary and supported only in Internet Explorer. Instead, [sync SharePoint files with the new OneDrive sync client](https://support.office.com/article/6de9ede8-5b6e-4503-80b2-6190f3354a88.aspx) which includes [Files On-Demand](https://support.office.com/article/0e6860d3-d9f3-4971-b321-7092438fb38e.aspx). Access all your files in OneDrive without using local storage space.</span></span>
  