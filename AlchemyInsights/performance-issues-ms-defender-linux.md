---
title: Linux 用 Microsoft Defender for Endpoint のパフォーマンスの問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: b1200f0dd206e27cccf96778beb0326c846e7504e51be283193b2630edfb4509
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54086745"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Linux 用 Microsoft Defender for Endpoint のパフォーマンスの問題

この記事では、Linux 上の Microsoft Defender for Endpoint のパフォーマンスの問題を特定する手順について説明します。

最初に、発生している問題が[最新バージョン](/microsoft-365/security/defender-endpoint/linux-whatsnew)で解決されていることを確認することが重要です。 

調査を開始するには、「[Linux用の Microsoft Defender for Endpoint のパフォーマンスの問題のトラブルシューティング](/microsoft-365/security/defender-endpoint/linux-support-perf)」 を参照してください。

## <a name="exclusions"></a>除外

除外は、パフォーマンスの問題を軽減するのに役立ちます。 開始する前に除外をレビューし、追加のリスクが認識されて文書化されるようにします。

詳細については、「[Linux 用の Microsoft Defender for Endpoint の除外を構成および検証する](/microsoft-365/security/defender-endpoint/linux-exclusions)」 を参照してください。

除外するファイルとフォルダーが複数あり、それらがすべて同じマウント ポイントにある場合は、マウントポイントを除外する方が簡単な場合があります。 2 月のリリース 101.22.80 以降では、マウントポイント全体を除外できます。

たとえば、/mnt/backup がマウントポイントの場合は、次のコマンドを実行して除外リストに /mnt/backup を追加できます。

`$ mdatp exclusion folder add –path /mnt/backup`

**注**: 除外を追加すると、マルウェアが検出されないリスクが高まるので、慎重に処理して実装する必要があります。

## <a name="need-help"></a>お困りですか?

最も効率的な方法で支援するには、サポート ケースを開く前に診断データを収集します。
