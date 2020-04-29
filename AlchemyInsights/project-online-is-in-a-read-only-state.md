---
title: Project Online が読み取り専用状態
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: dea4e24b0ceb0054f04e6737df0feb761d1143f3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43768010"
---
# <a name="project-online-is-in-a-read-only-state"></a><span data-ttu-id="cf118-102">Project Online が読み取り専用状態</span><span class="sxs-lookup"><span data-stu-id="cf118-102">Project Online is in a read-only state</span></span>

<span data-ttu-id="cf118-103">Project Online が読み取り専用状態になる共通の理由は 3 つあります。</span><span class="sxs-lookup"><span data-stu-id="cf118-103">There are three common reasons why Project Online may reach a read-only state:</span></span>

1. <span data-ttu-id="cf118-104">組織には、Project Online Essentials のライセンスのみがあります。</span><span class="sxs-lookup"><span data-stu-id="cf118-104">Organizations have a Project Online Essentials license(s) only.</span></span> <span data-ttu-id="cf118-105">これはサイトを維持させるのには不十分で、最終的にプロビジョニング解除されます。</span><span class="sxs-lookup"><span data-stu-id="cf118-105">This isn't enough to keep the site alive and it will eventually get de-provisioned.</span></span><span data-ttu-id="cf118-106">管理者が何かが間違っていることを認識し、正しいライセンスを取得できるように、サイトを読み取り専用状態にします。</span><span class="sxs-lookup"><span data-stu-id="cf118-106"> We place the site in a read-only state so that Admins know something is wrong and can acquire the correct licenses.</span></span> <span data-ttu-id="cf118-107">管理者は、Project Online Professional または Premium、あるいはその両方のライセンスを追加する必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf118-107">Admins will need to add a Project Online Professional and/or Premium license.</span></span> <span data-ttu-id="cf118-108">その時点でサイトは読み取り専用になります。</span><span class="sxs-lookup"><span data-stu-id="cf118-108">The site will come out of read-only at that point.</span></span> <span data-ttu-id="cf118-109">詳細については、「[プロジェクト管理解決策を比較する](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf118-109">For more info, see [Compare Project Management Solutions](https://products.office.com/project/compare-microsoft-project-management-software?tab=1).</span></span>
2. <span data-ttu-id="cf118-110">割り当てられたクォータに達しました。</span><span class="sxs-lookup"><span data-stu-id="cf118-110">Assigned quota has been reached.</span></span> <span data-ttu-id="cf118-111">詳細については、「[Project Web App クォータ](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)」を参照してください。 </span><span class="sxs-lookup"><span data-stu-id="cf118-111">For more info, see [Project Web App Quota](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota).</span></span> <span data-ttu-id="cf118-112">レポートの精密性がクォータの使用状況にどのように影響するかを確認するには、「[Project Online で時間配分レポート データの重ね合わせを構成する](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online)」を確認します。</span><span class="sxs-lookup"><span data-stu-id="cf118-112">Check [Configure rollup of timephased reporting data in Project Online](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online) to see how reporting granularity may impact quota usage.</span></span>
3. <span data-ttu-id="cf118-113">読み取り専用は、メンテナンス中に発生する可能性がある非常に一時的な状態です。</span><span class="sxs-lookup"><span data-stu-id="cf118-113">Read-only can be a very temporary condition that can occur during maintenance.</span></span> <span data-ttu-id="cf118-114">ほとんどのメンテナンスは顧客には気づかれず、しばしばこれを見ることはないですが、短期間の読み取り専用を経験する時があります。</span><span class="sxs-lookup"><span data-stu-id="cf118-114">Most maintenance is not even noticed by our customers and you will not often see this, but there are times when short periods of read-only are experienced.</span></span>
