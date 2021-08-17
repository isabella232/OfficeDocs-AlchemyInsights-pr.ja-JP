---
title: Windows Virtual Desktop 用のサービス診断ツール
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: 58688e3216ba6777b1a4f76095bd39c81a2d2a8294e06b6bc61c7134f6d589f9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052391"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Windows Virtual Desktop 用のサービス診断ツール

Windows Virtual Desktop (WVD) は、管理者が単一のインターフェイスを介してエラーを識別できるようにする診断ツールを提供します。 このツールは、WVD の役割が割り当てられた誰かが WVD を使用するたびに、診断関連の情報をログに記録します。 各ログには、アクティビティに関係する WVD 役割に関する情報、セッション中に表示されるエラー メッセージ、およびテナントとユーザーに関する情報が含まれます。 Azure Log Analytics は、診断ツールによって作成されたアクティビティ ログをキャプチャするように構成できます。 次の操作を実行してください。

1. [Azure ポータル](https://go.microsoft.com/fwlink/?linkid=2129500)または [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501) を使用して Log Analytics ワークスペースを作成します。
1. [Windows コンピューターを Azure Monitor](https://go.microsoft.com/fwlink/?linkid=2129913) に接続します。 ワークスペース ID とワークスペースの主キーを取得します。 セットアップ ウィザードは、エージェントを適切に構成し、Azure Monitor と通信できるようにするためにこの情報を必要とします。
1. [診断データをワークスペースにプッシュします](https://go.microsoft.com/fwlink/?linkid=2128284)。 WVD テナントからワークスペースの Log Analytics に診断データをプッシュできます。
1. WVD に関連して内部または外部にある[問題を特定して診断します](https://go.microsoft.com/fwlink/?linkid=2128338)。

WVD のサービス診断ツールの構成の詳細については、「[診断機能に Log Analytics を使用する](https://go.microsoft.com/fwlink/?linkid=2128084)」を参照してください。
