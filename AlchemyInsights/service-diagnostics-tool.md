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
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktop 用のサービス診断ツール

Windows Virtual Desktop (WVD) は、管理者が単一のインターフェイスを介してエラーを識別できるようにする診断ツールを提供します。 このツールは、WVD の役割が割り当てられた誰かが WVD を使用するたびに、診断関連の情報をログに記録します。 各ログには、アクティビティに関係する WVD 役割に関する情報、セッション中に表示されるエラー メッセージ、およびテナントとユーザーに関する情報が含まれます。 Azure Log Analytics は、以下の手順に従うことにより、診断ツールによって作成されたアクティビティ ログをキャプチャするように構成できます。

1. [Azure ポータル](https://go.microsoft.com/fwlink/?linkid=2129500)または [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) を使用して Log Analytics ワークスペースを作成します。

1. [Windows コンピューターを Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913) に接続します。 ワークスペース ID とワークスペースの主キーを取得します。 セットアップ ウィザードは、エージェントを適切に構成し、Azure Monitor と通信できるようにするためにこの情報を必要とします。

1. [診断データをワークスペースにプッシュします](https://go.microsoft.com/fwlink/?linkid=2128284)。 WVD テナントからワークスペースの Log Analytics に診断データをプッシュできます。

1. WVD に関連して内部または外部にある問題を[特定して診断](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)します。

WVD のサービス診断ツールの構成の詳細については、「診断機能に Log Analytics を使用する」を参照してください。