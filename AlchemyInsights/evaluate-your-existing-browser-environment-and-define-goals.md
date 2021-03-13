---
title: 既存のブラウザー環境を評価し、目標を定義する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9141"
- "9005291"
ms.openlocfilehash: 5b03d188aa78be83928cf262f1d86f3f933c85ab
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696433"
---
# <a name="evaluate-your-existing-browser-environment-and-define-goals"></a><span data-ttu-id="67ebd-102">既存のブラウザー環境を評価し、目標を定義する</span><span class="sxs-lookup"><span data-stu-id="67ebd-102">Evaluate your existing browser environment and define goals</span></span>

<span data-ttu-id="67ebd-103">時間をかけて現在のブラウザーの状態とプロジェクトのビジョンを理解することで、すべてのプロジェクト関係者が一致して、同じ目標に向けて取り組むことができます。</span><span class="sxs-lookup"><span data-stu-id="67ebd-103">Taking time to understand your current browser state and project vision ensures all project stakeholders are aligned and are working toward the same goal.</span></span> <span data-ttu-id="67ebd-104">次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="67ebd-104">Follow these steps:</span></span>

1. <span data-ttu-id="67ebd-105">現在の状態を定義する。</span><span class="sxs-lookup"><span data-stu-id="67ebd-105">Define your current state.</span></span> <span data-ttu-id="67ebd-106">次の状況について検討しましょう。</span><span class="sxs-lookup"><span data-stu-id="67ebd-106">Consider the following:</span></span>
- <span data-ttu-id="67ebd-107">現在、どのブラウザーが環境に展開されていますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-107">Which browsers are currently deployed in your environment?</span></span>
- <span data-ttu-id="67ebd-108">どのブラウザーが既定のブラウザーとして設定されていますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-108">Which browser is set as the default browser?</span></span>
- <span data-ttu-id="67ebd-109">一部のアプリで Internet Explorer を使用する必要がありますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-109">Do you need to use Internet Explorer for some of your apps?</span></span>
- <span data-ttu-id="67ebd-110">エンタープライズ モード のサイト リストを使用して、現在使っている Internet Explorer を構成していますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-110">Do you use an Enterprise Mode Site List to configure Internet Explorer today?</span></span>
- <span data-ttu-id="67ebd-111">お使いの環境でサポートされている OS プラットフォーム(Windows 10やmacOSなど)はどれですか？ </span><span class="sxs-lookup"><span data-stu-id="67ebd-111">Which OS platforms, such as Windows 10 and macOS, does your environment support?</span></span>
- <span data-ttu-id="67ebd-112">ブラウザー管理には、どの管理ツールを使用しますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-112">Which management tools do you use for browser management?</span></span>
- <span data-ttu-id="67ebd-113">ブラウザーの構成と管理の責任者</span><span class="sxs-lookup"><span data-stu-id="67ebd-113">Who's responsible for browser configuration and management?</span></span>
- <span data-ttu-id="67ebd-114">ブラウザーの互換性を検証するためのプロセス</span><span class="sxs-lookup"><span data-stu-id="67ebd-114">What's the process for validating browser compatibility?</span></span>
2. <span data-ttu-id="67ebd-115">展開の目標を定義する。</span><span class="sxs-lookup"><span data-stu-id="67ebd-115">Define the goals for your deployment.</span></span> <span data-ttu-id="67ebd-116">以下の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="67ebd-116">Keep the following things in mind:</span></span>
- <span data-ttu-id="67ebd-117">[Microsoft Edge を既定のブラウザー アカウントとして設定](https://docs.microsoft.com/DeployEdge/edge-default-browser)しますか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-117">Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/DeployEdge/edge-default-browser)?</span></span>
- <span data-ttu-id="67ebd-118">レガシ バージョンの Microsoft Edge を非表示にしますか? それとも、[ユーザーが引き続き使用できるようにします](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)か?</span><span class="sxs-lookup"><span data-stu-id="67ebd-118">Do you want to hide the legacy version of Microsoft Edge or do you want to [leave it available for users](https://docs.microsoft.com/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?</span></span>
- <span data-ttu-id="67ebd-119">[Microsoft Edge の構成方法](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)。</span><span class="sxs-lookup"><span data-stu-id="67ebd-119">How will you [configure Microsoft Edge](https://docs.microsoft.com/DeployEdge/configure-microsoft-edge)?</span></span>
- <span data-ttu-id="67ebd-120">初期展開の一環として、構成する上で重要な機能は何ですか?</span><span class="sxs-lookup"><span data-stu-id="67ebd-120">What features are critical to configure as part of your initial deployment?</span></span>
- <span data-ttu-id="67ebd-121">特定された互換性や構成の問題に対処するためのプロセス</span><span class="sxs-lookup"><span data-stu-id="67ebd-121">What is the process for addressing any identified compatibility or configuration issues?</span></span>
3. <span data-ttu-id="67ebd-122">次のような、使用する機能の前提条件を理解します。</span><span class="sxs-lookup"><span data-stu-id="67ebd-122">Understand the prerequisites for features you might want to use, such as:</span></span>
- [<span data-ttu-id="67ebd-123">Windows Defender Application Guard</span><span class="sxs-lookup"><span data-stu-id="67ebd-123">Windows Defender Application Guard</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-application-guard/reqs-md-app-guard)
- [<span data-ttu-id="67ebd-124">Internet Explorer モード</span><span class="sxs-lookup"><span data-stu-id="67ebd-124">Internet Explorer mode</span></span>](https://docs.microsoft.com/DeployEdge/edge-ie-mode)
- [<span data-ttu-id="67ebd-125">認証と同期</span><span class="sxs-lookup"><span data-stu-id="67ebd-125">Authentication and sync</span></span>](https://docs.microsoft.com/DeployEdge/microsoft-edge-security-identity)

<span data-ttu-id="67ebd-126">これらの手順を完了したら、展開戦略の計画を開始する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="67ebd-126">After you complete these steps, you're ready to start planning your deployment strategy.</span></span>
