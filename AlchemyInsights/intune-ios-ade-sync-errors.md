---
title: Apple デバイスの自動登録同期エラー
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013753"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple デバイスの自動登録同期エラー

「エラー状態にある 1 つまたは複数の ADE/DEP トークンがあることを検出しました。 影響を受ける各トークンについてエラーの状態が解決されるまで、ADE 機能は期待どおりに使用できません。」

このエラーは、次のような場合に表示されることがあります。

1. デバイスが ABM/ASM から Intune に同期されないことがある
2. 登録プロファイルの割り当てが失敗した可能性がある
3. デバイスが ADE 登録を正常に完了しないことがある

**[デバイス]、[デバイスの登録]、[Apple の登録]、[登録プログラムのトークン]** の順に Intune コンソールに報告された同期エラーがあるか確認します。

同期エラーの最も一般的な原因の 1 つは、現在のトークンの有効期限です。 多くの場合、影響を受けるトークンを更新すると問題が解決します。

1 つ以上のトークンの有効期限が切れている場合は、次のドキュメントを参照して必要に応じてトークンを更新します。

[自動デバイス登録トークンを更新する](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

さらに、次のドキュメントを参照して、トークンの同期エラーの原因となる他のエラーの潜在的な修正を確認できます。

[IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[IOS/iPadOS および macOS の自動デバイスの登録トークンの ABM/ASM 同期エラー](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
