---
title: DataProtection-Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/30/2019
ms.locfileid: "40923551"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune で Bitlocker 暗号化を有効にする

 Intune Endpoint Protection ポリシーを使用して、Windows デバイスの Bitlocker 暗号化設定を構成できます。 詳細については、「 [Windows 10 以降の設定」の「Intune を使用してデバイスを保護する](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)」を参照してください。
 
Windows 10 を実行している新しいデバイスの多くは、自動 Bitlocker 暗号化をサポートしていますが、これは MDM ポリシーの適用なしでトリガーされることに注意してください。 既定以外の設定が構成されている場合、ポリシーの適用に影響する可能性があります。 詳細については、次の FAQ を参照してください。
 
Bitlocker の問題のトラブルシューティングの詳細については、「 [Microsoft Intune での bitlocker ポリシーのトラブルシューティング](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)」を参照してください。
 
 
**FAQ**

 Q: エンドポイント保護ポリシーを使用してデバイスの暗号化をサポートしている Windows のエディションを教えてください。<br>
 A: Intune Endpoint Protection ポリシーの設定は、 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)を使用して実装されています。 Windows のすべてのエディションまたはビルドが Bitlocker CSP をサポートするわけではありません。 <br><br>
      現時点では、次の Windows エディションがサポートされています。 Enterprise、エデュケーション、Mobile、Mobile Enterprise、Professional (ビルド1809以降)。
 
Q: 暗号化方式と暗号強度 (XTS-128) の OS の既定の設定を使用して、デバイスが既に Bitlocker で暗号化されている場合、別の設定のポリシーを適用すると、新しい設定でドライブの再暗号化が自動的にトリガーされますか。<br>
A: いいえ。 新しい cipher 設定を適用するには、最初にドライブを復号化する必要があります。<br><br>
**注:** 自動操縦によって登録されているデバイスの場合、OOBE 中に発生する自動暗号化は、Intune ポリシーが評価されるまでトリガーされないため、ポリシーベースの設定を OS の既定値の代わりに使用できます。
 
Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されると、暗号化が解除されますか。<br>
A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号化が解除されることはありません。
 
Q: Intune コンプライアンスポリシーが、Bitlocker が有効になっていないのに、Bitlocker が有効になっていないことを示しているのはなぜですか?<br>
A: Intune コンプライアンスポリシーの "Bitlocker enabled" 設定は、Windows デバイス正常性構成証明 (DHA) クライアントを利用します。 このクライアントは、ブート時のデバイスの状態のみ評価します。 Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアントサービスは Bitlocker をアクティブとして報告しません。
 
 