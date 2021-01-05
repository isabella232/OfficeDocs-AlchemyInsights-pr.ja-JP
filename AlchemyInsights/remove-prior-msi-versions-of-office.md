---
title: 以前の MSI バージョンの Office を削除する
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 26ab610cb204149536bd23c830a1b8558892a7c0
ms.sourcegitcommit: c033720921cb9a06b9560eedef4f1935e69a846b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2020
ms.locfileid: "49680799"
---
# <a name="remove-prior-msi-versions-of-office"></a><span data-ttu-id="23a69-102">以前の MSI バージョンの Office を削除する</span><span class="sxs-lookup"><span data-stu-id="23a69-102">Remove prior MSI versions of Office</span></span>

<span data-ttu-id="23a69-103">Office 365 ProPlus をインストールする前に、以前の Windows インストーラー (MSI) 版の Office を削除することをおすすめします。</span><span class="sxs-lookup"><span data-stu-id="23a69-103">I recommend removing prior Windows Installer (MSI) versions of Office before installing Office 365 ProPlus.</span></span> <span data-ttu-id="23a69-104">その手順は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="23a69-104">Here's how to do this:</span></span>

1. <span data-ttu-id="23a69-105">MSI を使用して Office をインストールした場合は、Office 展開ツール (ODT) を使用して Office をアンインストールできます。</span><span class="sxs-lookup"><span data-stu-id="23a69-105">If you used MSI to install Office, you can use the Office Deployment Tool (ODT) to uninstall Office.</span></span> <span data-ttu-id="23a69-106">RemoveMSI element は、**configuration.xml** ファイルで使用できます。</span><span class="sxs-lookup"><span data-stu-id="23a69-106">You can use the RemoveMSI element in your **configuration.xml** file.</span></span>
1. <span data-ttu-id="23a69-107">この記事 ([Office 365 セキュリティ/コンプライアンス センター](https://go.microsoft.com/fwlink/p/?linkid=2077143)) の手順に従います。</span><span class="sxs-lookup"><span data-stu-id="23a69-107">Follow the instruction in this article: [Office 365 Security & Compliance Center.](https://go.microsoft.com/fwlink/p/?linkid=2077143)</span></span>