---
title: Project Online が読み取り専用状態
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 4/10/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: 34fecf93f39659cbd26998697090957c6af45aa0
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054364"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="d5a01-102">Project Online が読み取り専用状態</span><span class="sxs-lookup"><span data-stu-id="d5a01-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="d5a01-103">Project Online が読み取り専用状態になる共通の理由は 3 つあります。</span><span class="sxs-lookup"><span data-stu-id="d5a01-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="d5a01-104">組織には、Project Online Essentials のライセンスのみがあります。</span><span class="sxs-lookup"><span data-stu-id="d5a01-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="d5a01-105">これはサイトを維持させるのには不十分で、最終的にプロビジョニング解除されます。</span><span class="sxs-lookup"><span data-stu-id="d5a01-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="d5a01-106">管理者が何かが間違っていることを認識し、正しいライセンスを取得できるように、サイトを読み取り専用状態にします。</span><span class="sxs-lookup"><span data-stu-id="d5a01-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="d5a01-107">管理者は、Project Online Professional または Premium、あるいはその両方のライセンスを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5a01-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="d5a01-108">その時点でサイトは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="d5a01-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="d5a01-109">詳細については、「[プロジェクト管理解決策を比較する](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d5a01-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="d5a01-110">割り当てられたクォータに達しました。</span><span class="sxs-lookup"><span data-stu-id="d5a01-110">Assigned quota has been reached.</span></span> <span data-ttu-id="d5a01-111">詳細については、「[Project Web App クォータ](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)」を参照してください。 </span><span class="sxs-lookup"><span data-stu-id="d5a01-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="d5a01-112">レポートの精密性がクォータの使用状況にどのように影響するかを確認するには、「[Project Online で時間配分レポート データの重ね合わせを構成する](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online?redirectSourcePath=%252fen-us%252farticle%252fConfigure-rollup-of-timephased-reporting-data-in-Project-Online-da8487fe-899e-4510-a264-e2ebc948928c)」を確認します。</span><span class="sxs-lookup"><span data-stu-id="d5a01-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online?redirectSourcePath=%252fen-us%252farticle%252fConfigure-rollup-of-timephased-reporting-data-in-Project-Online-da8487fe-899e-4510-a264-e2ebc948928c) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="d5a01-113">読み取り専用は、メンテナンス中に発生する可能性がある非常に一時的な状態です。</span><span class="sxs-lookup"><span data-stu-id="d5a01-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="d5a01-114">ほとんどのメンテナンスは顧客には気づかれず、しばしばこれを見ることはないですが、短期間の読み取り専用を経験する時があります。</span><span class="sxs-lookup"><span data-stu-id="d5a01-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
