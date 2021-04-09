---
title: Windows Virtual Desktop 用のサービス診断ツール
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10873"
ms.openlocfilehash: dfa59c86508c8658c880f4f3f21a002524e909d1
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/05/2021
ms.locfileid: "51596097"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a><span data-ttu-id="9f826-102">Windows Virtual Desktop 用のサービス診断ツール</span><span class="sxs-lookup"><span data-stu-id="9f826-102">Service diagnostics tool for Windows Virtual Desktop</span></span>

<span data-ttu-id="9f826-103">Windows Virtual Desktop (WVD) は、管理者が単一のインターフェイスを介してエラーを識別できるようにする診断ツールを提供します。</span><span class="sxs-lookup"><span data-stu-id="9f826-103">Windows Virtual Desktop (WVD) offers a diagnostic tool that lets admins identify errors through a single interface.</span></span> <span data-ttu-id="9f826-104">このツールは、WVD の役割が割り当てられた誰かが WVD を使用するたびに、診断関連の情報をログに記録します。</span><span class="sxs-lookup"><span data-stu-id="9f826-104">This tool logs diagnostics-related info whenever WVD is used by someone assigned a WVD role.</span></span> <span data-ttu-id="9f826-105">各ログには、アクティビティに関係する WVD 役割に関する情報、セッション中に表示されるエラー メッセージ、およびテナントとユーザーに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="9f826-105">Each log contains info about the WVD role involved in the activity, the error messages that appear during the session, and the info about the tenant and user.</span></span> <span data-ttu-id="9f826-106">Azure Log Analytics は、以下の手順に従うことにより、診断ツールによって作成されたアクティビティ ログをキャプチャするように構成できます。</span><span class="sxs-lookup"><span data-stu-id="9f826-106">Azure Log Analytics can be configured to capture the activity log created by the diagnostic tool by following these steps:</span></span>

1. <span data-ttu-id="9f826-107">[Azure ポータル](https://go.microsoft.com/fwlink/?linkid=2129500)または [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) を使用して Log Analytics ワークスペースを作成します。</span><span class="sxs-lookup"><span data-stu-id="9f826-107">Create a Log Analytics workspace with the [Azure portal](https://go.microsoft.com/fwlink/?linkid=2129500) or [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).</span></span>

1. <span data-ttu-id="9f826-108">[Windows コンピューターを Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913) に接続します。</span><span class="sxs-lookup"><span data-stu-id="9f826-108">[Connect Windows computers to Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913).</span></span> <span data-ttu-id="9f826-109">ワークスペース ID とワークスペースの主キーを取得します。</span><span class="sxs-lookup"><span data-stu-id="9f826-109">Get the Workspace ID and the Primary Key of your workspace.</span></span> <span data-ttu-id="9f826-110">セットアップ ウィザードは、エージェントを適切に構成し、Azure Monitor と通信できるようにするためにこの情報を必要とします。</span><span class="sxs-lookup"><span data-stu-id="9f826-110">The setup wizard needs this info to properly configure the agent and to ensure it can communicate with Azure Monitor.</span></span>

1. <span data-ttu-id="9f826-111">[診断データをワークスペースにプッシュします](https://go.microsoft.com/fwlink/?linkid=2128284)。</span><span class="sxs-lookup"><span data-stu-id="9f826-111">[Push diagnostics data to your workspace](https://go.microsoft.com/fwlink/?linkid=2128284).</span></span> <span data-ttu-id="9f826-112">WVD テナントからワークスペースの Log Analytics に診断データをプッシュできます。</span><span class="sxs-lookup"><span data-stu-id="9f826-112">You can push diagnostics data from your WVD tenant to the Log Analytics for your workspace.</span></span>

1. <span data-ttu-id="9f826-113">WVD に関連して内部または外部にある問題を[特定して診断](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)します。</span><span class="sxs-lookup"><span data-stu-id="9f826-113">[Identify and diagnose](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell) issues that are internal or external in relation to WVD.</span></span>

<span data-ttu-id="9f826-114">WVD のサービス診断ツールの構成の詳細については、「診断機能に Log Analytics を使用する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f826-114">To learn more about configuring the service diagnostics tool for WVD, see Use Log Analytics for the diagnostics feature.</span></span>