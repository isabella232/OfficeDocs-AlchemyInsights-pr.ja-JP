---
title: 'エラー: このコンピューターのルールは一致しません'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c0982da82826d1644f437b19e0d343a59d7ac473
ms.sourcegitcommit: e09af4285c6b81ca0a5320fdb811713ac25748c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/09/2020
ms.locfileid: "44664251"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="2a937-102">エラー: このコンピューターのルールは一致しません</span><span class="sxs-lookup"><span data-stu-id="2a937-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="2a937-103">この既知の問題の最新の状態を確認するには、「[このコンピューターのルールが Microsoft Exchange のルールと一致しない](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a937-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="2a937-104">Outlook チームは、ビルド 12928.10000 で修正プログラムを実装しました。</span><span class="sxs-lookup"><span data-stu-id="2a937-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="2a937-105">この修正プログラムは既に Insider ファーストで利用できます。また、2020 年 6 月後半には、月次チャネルでも利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="2a937-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="2a937-106">修正プログラムのビルドが完了すると、「保持したいルールを選んでください」というメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a937-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="2a937-107">メッセージが表示されたら、[サーバー] を選んでから、Outlook に戻り、無効になっていたルールを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="2a937-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="2a937-108">修正プログラムが使用可能になるまで、次の回避策を使用してください。</span><span class="sxs-lookup"><span data-stu-id="2a937-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="2a937-109">**回避策**: 最新のレポートでは、Outlook デスクトップでクライアント ルールを作成しただけのユーザーにこの問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="2a937-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="2a937-110">問題の発生が続く場合は、該当のルールを削除してから、OWA (Outlook Web App) で、問題が解消するまでルールを作成、編集します。</span><span class="sxs-lookup"><span data-stu-id="2a937-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="2a937-111">ルールを手動で削除できない場合は、Outlook を起動する時にOutlook.exe /cleanrules を実行することで Outlook のコマンドを実行できます。</span><span class="sxs-lookup"><span data-stu-id="2a937-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="2a937-112">これにより、クライアントとサーバー両方のルールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="2a937-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="2a937-113">Outlook プロファイル内すべてのアカウントの全ルールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="2a937-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="2a937-114">このコマンドについては詳しくは、コマンド ライン スイッチの記事に記載されています。</span><span class="sxs-lookup"><span data-stu-id="2a937-114">This command is further documented in the Command-line switches article.</span></span>

