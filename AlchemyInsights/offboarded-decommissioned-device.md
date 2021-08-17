---
title: オフボードまたは廃止されたデバイスをデバイス インベントリから削除する場合の問題点
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/11/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002913"
- "11187"
ms.openlocfilehash: 814301e9cd8197e62dcca68ab3bdde1618d210f73a744b53bb5af7b861eb02bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54076657"
---
# <a name="issues-with-removing-an-offboarded-or-decommissioned-device-from-the-device-inventory"></a>オフボードまたは廃止されたデバイスをデバイス インベントリから削除する場合の問題点

Microsoft Defender for Endpoint では現在、オフボードまたは使用を停止したデバイスのデバイス レコードをデバイス インベントリから手動で削除することはできません。

セキュリティ上の理由から、デバイスは最大 180 日間、履歴としてポータルに残ります。 ただし、デバイス データは、設定した保存期間に従って消去されます。

**注**: オフボードまたは使用を停止したデバイスは、7 日後に自動的に **非アクティブ** 状態に切り替わります。 また、過去 30 日間にアクティブでなかったデバイスは、組織の脅威と脆弱性管理の公開スコアやデバイス向けの Microsoft セキュリティ スコアを反映するデータには反映されません。
 
それでも特定のデバイスがデバイス インベントリ ビューに表示されない場合は、デバイス タグを配置して、デバイス インベントリ ビューから使用を停止したデバイスのフィルター処理をお試しください。

詳細については、以下を参照してください。

[Microsoft Defender for Endpoint サービスのオフボード デバイス](/microsoft-365/security/defender-endpoint/offboard-machines.md)

[脅威と脆弱性の管理における露出スコア](/microsoft-365/security/defender-endpoint/tvm-exposure-score.md)

[Microsoft Defender for Endpoint で問題が発生したセンサーの修正](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors#inactive-devices.md)

[タグの効果的な使用方法 (パート 1)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-1/ba-p/1964058)

[タグの効果的な使用方法 (パート 2)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-2/ba-p/1962008)

[タグの効果的な使用方法 (パート 3)](https://techcommunity.microsoft.com/t5/microsoft-defender-for-endpoint/how-to-use-tagging-effectively-part-3/ba-p/1964073)




