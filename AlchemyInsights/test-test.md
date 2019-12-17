---
title: SharePoint Online 用語ストアで用語が見つからない
ms.author: pebaum
author: pebaum
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 28913b8e57e39d51e8957b7408c19337a119c589
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053518"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune で Bitlocker 暗号化を有効にする

Intune のエンドポイント保護ポリシーは、「Intune を使用してデバイスを保護するための Windows 10 (以降) の設定」に記載されているように、Windows デバイスの Boitlocker 暗号化の設定を構成するために使用できます

Windows 10 を実行する多くの新しいデバイスでは、MDM ポリシーの適用なしでトリガーされる自動 Boitlocker 暗号化をサポートしていることを、ユーザーは認識する必要があります。 これは、非既定の設定が構成されている場合、ポリシーの適用に影響を与える可能性があります。 詳細については、FAQ を参照してください。


FAQ  Q: エンドポイント保護ポリシーを使用するデバイスの暗号化をサポートする Windows のエディションはどれですか?
 A: Intune エンドポイント保護ポリシーの設定は、Bitlocker CSP を使用して実装されています。すべての Windows のエディションやビルドで Bitlocker CSP をサポートしているわけではありません。 
      現時点の Windows エディション: Enterprise、Education、Mobile、Mobile Enterprise および Professional (ビルド 1809 以降) がサポートされています。




Q: デバイスが、暗号化方法と暗号強度 (XTS-AES-128)  に対する OS の既定の設定を使用している Bitlocker で暗号化されている場合、新しい設定を使用してドライブの再暗号化を自動でトリガーできる、設定の異なるポリシーを適用することはできますか?

A: いいえ。 新しい暗号の設定を適用するために、ドライブの暗号化を最初に解除する必要があります。

注: OOBE 中に行われる Autopilot の自動暗号化を使用してデバイスが登録されている場合は、OS の既定値の代わりに使用されるポリシー ベースの設定を許可する Intune ポリシーが評価されるまで、トリガーされません。




Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されれば、デバイスの暗号は解除されますか?

A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号は解除されません。




Q: Intune コンプライアンス ポリシーで、デバイスは "Bitlocker 有効" な状態ではありませんと表示されるのはどうしてですか?

A: Intune コンプライアンス ポリシーの "Bitlocker 有効" の設定では、 Windows デバイス正常性構成証明 (DHA) のクライアントを利用します。 このクライアントは、ブート時のデバイスの状態のみ評価します。 そのため、Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアント サービスでは Bitlocker をアクティブな状態として報告しません。