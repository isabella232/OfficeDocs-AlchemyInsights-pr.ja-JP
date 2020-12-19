---
title: Apple デバイスの自動登録同期エラー
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: d7a9398046a1073e30fdbe2950f750bb55d4fa2f
ms.sourcegitcommit: 87c8d0a1e6668211b9dd5427f98984ccdcadb02d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/17/2020
ms.locfileid: "49715069"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple デバイスの自動登録同期エラー

「エラー状態にある 1 つまたは複数の ADE/DEP トークンがあることを検出しました。 影響を受ける各トークンについてエラーの状態が解決されるまで、ADE 機能は同様に使用できません。」

このエラーは、次のような場合に表示されることがあります。

1. デバイスが ABM/ASM から Intune に同期されないことがある
2. 登録プロファイルの割り当てが失敗した可能性がある
3. デバイスが ADE 登録を正常に完了しないことがある

**[デバイス]、 [デバイスの登録]、[ Apple の登録]、 [登録プログラムのトークン]** の順に Intune コンソールに報告された同期エラーがあるか確認して、可能性のある改善策を以下のドキュメントを参照し確認します。

[IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
