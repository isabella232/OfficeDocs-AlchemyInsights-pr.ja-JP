---
title: 'エラー: このコンピューターのルールは一致しません'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690968"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="c042f-102">エラー: このコンピューターのルールは一致しません</span><span class="sxs-lookup"><span data-stu-id="c042f-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="c042f-103">この既知の問題の最新の状態を確認するには、「[このコンピューターのルールが Microsoft Exchange のルールと一致しない](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c042f-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="c042f-104">Outlook チームは、ビルド 12928.10000 で修正プログラムを実装しました。</span><span class="sxs-lookup"><span data-stu-id="c042f-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="c042f-105">この修正プログラムは既に Insider ファーストで利用できます。また、2020 年 6 月後半には、月次チャネルでも利用可能になります。</span><span class="sxs-lookup"><span data-stu-id="c042f-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="c042f-106">修正プログラムのビルドが完了すると、「保持したいルールを選んでください」というメッセージが表示される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c042f-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="c042f-107">メッセージが表示されたら、[サーバー] を選んでから、Outlook に戻り、無効になっていたルールを再び有効にします。</span><span class="sxs-lookup"><span data-stu-id="c042f-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="c042f-108">修正プログラムが使用可能になるまで、次の回避策を使用してください。</span><span class="sxs-lookup"><span data-stu-id="c042f-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="c042f-109">**回避策**: 最新のレポートでは、Outlook デスクトップでクライアント ルールを作成しただけのユーザーにこの問題が発生しています。</span><span class="sxs-lookup"><span data-stu-id="c042f-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="c042f-110">問題の発生が続く場合は、該当のルールを削除してから、OWA (Outlook Web App) で、問題が解消するまでルールを作成、編集します。</span><span class="sxs-lookup"><span data-stu-id="c042f-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="c042f-111">ルールを手動で削除できない場合は、Outlook を起動する時にOutlook.exe /cleanrules を実行することで Outlook のコマンドを実行できます。</span><span class="sxs-lookup"><span data-stu-id="c042f-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="c042f-112">これにより、クライアントとサーバー両方のルールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="c042f-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="c042f-113">Outlook プロファイル内すべてのアカウントの全ルールが削除されます。</span><span class="sxs-lookup"><span data-stu-id="c042f-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="c042f-114">このコマンドについては詳しくは、コマンド ライン スイッチの記事に記載されています。</span><span class="sxs-lookup"><span data-stu-id="c042f-114">This command is further documented in the Command-line switches article.</span></span>

