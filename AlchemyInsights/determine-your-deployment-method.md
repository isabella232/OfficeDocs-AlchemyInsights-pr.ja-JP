---
title: 展開方法を決定する
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
- "9142"
- "9005291"
ms.openlocfilehash: 149fd99d1c8e62e568e1e8fbff87ab00fba86f76
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2021
ms.locfileid: "50696437"
---
# <a name="determine-your-deployment-method"></a><span data-ttu-id="ceedb-102">展開方法を決定する</span><span class="sxs-lookup"><span data-stu-id="ceedb-102">Determine your deployment method</span></span>

<span data-ttu-id="ceedb-103">展開の目標が定義されたので、次に計画を立て始めてください。</span><span class="sxs-lookup"><span data-stu-id="ceedb-103">Now that you've defined the goals of your deployment, it's time to start planning.</span></span> <span data-ttu-id="ceedb-104">最初に、展開方法を決定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ceedb-104">First, you need to determine your deployment method.</span></span> <span data-ttu-id="ceedb-105">Microsoft Edge をユーザーに展開する主な方法には、役割別の展開とサイト別の展開の 2 つがあります。</span><span class="sxs-lookup"><span data-stu-id="ceedb-105">The two main ways to deploy Microsoft Edge to your users is by role or by site.</span></span>

<span data-ttu-id="ceedb-106">**役割別の展開**</span><span class="sxs-lookup"><span data-stu-id="ceedb-106">**Deploy by role**</span></span>

<span data-ttu-id="ceedb-107">役割別の展開は、各フェーズで発生する問題を見つけて修正できるので、複数のフェーズで展開する場合に最適です。</span><span class="sxs-lookup"><span data-stu-id="ceedb-107">Deploying by role is best if you want to deploy in phases, as you can find and fix issues that come up in each phase.</span></span> <span data-ttu-id="ceedb-108">アプリの互換性について質問がある場合、または完全な互換性テストを実行できない場合は、この方法をお選びください。</span><span class="sxs-lookup"><span data-stu-id="ceedb-108">If you have questions about app compatibility or are unable to do thorough compatibility testing, this is the preferred method.</span></span>

<span data-ttu-id="ceedb-109">**サイト別の展開**</span><span class="sxs-lookup"><span data-stu-id="ceedb-109">**Deploy by site**</span></span>

<span data-ttu-id="ceedb-110">次のシナリオでは、サイト別の展開が最適です。</span><span class="sxs-lookup"><span data-stu-id="ceedb-110">Deploying by site is best in the following scenarios:</span></span>
- <span data-ttu-id="ceedb-111">Microsoft Edge を迅速に展開したい場合で、効率を重視して、発生する問題は無視する場合</span><span class="sxs-lookup"><span data-stu-id="ceedb-111">If you want to get Microsoft Edge deployed quickly and aren't concerned about issues that come up, affecting efficiency</span></span>
- <span data-ttu-id="ceedb-112">広範なアプリの互換性テストは既に完了しています。</span><span class="sxs-lookup"><span data-stu-id="ceedb-112">You've already completed extensive app compatibility testing.</span></span> <span data-ttu-id="ceedb-113">また、この方法では、ソフトウェア配信の最適化も利用できます。</span><span class="sxs-lookup"><span data-stu-id="ceedb-113">This method also lets you take advantage of software delivery optimizations.</span></span>

<span data-ttu-id="ceedb-114">Microsoft Edge を展開する方法を選んだら、サイト検出を行って現在の環境をさらに定義する準備が整います。</span><span class="sxs-lookup"><span data-stu-id="ceedb-114">Once you've picked a method for deploying Microsoft Edge, you're ready to do site discovery to further define your current environment.</span></span>
