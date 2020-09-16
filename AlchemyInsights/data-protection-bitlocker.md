---
title: DataProtection - Bitlocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731244"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a>Intune で Bitlocker 暗号化を有効にする

 Intune エンドポイント保護ポリシーを使用して、Windows デバイスの BitLocker 暗号化設定を構成できます。 詳細については、「[Intune を使用してデバイスを保護する Windows 10 以降の設定](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)」を参照してください。
 
Windows 10 を実行する多くの新しいデバイスでは、MDM ポリシーの適用なしでトリガーされる自動 Bitlocker 暗号化をサポートしていることを、ユーザーは認識する必要があります。 これは、非既定の設定が構成されている場合、ポリシーの適用に影響を与える可能性があります。 詳細については、次の FAQ を参照してください。
 
Bitlocker の問題のトラブルシューティングについては、「[Microsoft Intune の BitLocker ポリシーのトラブルシューティング](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)」を参照してください。
 
 
**FAQ**

 Q: エンドポイント保護ポリシーを使用するデバイスの暗号化をサポートする Windows のエディションはどれですか?<br>
 A: Intune エンドポイント保護ポリシーの設定は、[Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp) を使用して実装されています。 すべての Windows のエディションまたはビルドで Bitlocker CSP をサポートしているわけではありません。 <br><br>
      現時点では、次の Windows エディションがサポートされています。Enterprise、Education、Mobile、Mobile Enterprise および Professional (ビルド 1809 以降)。
 
Q: デバイスが、暗号化方法と暗号強度 (XTS-AES-128) に対する OS の既定の設定を使用している Bitlocker で暗号化されている場合、新しい設定を使用してドライブの再暗号化を自動でトリガーできる、設定の異なるポリシーを適用することはできますか?<br>
A: いいえ。 新しい暗号の設定を適用するには、ドライブの暗号化を最初に解除する必要があります。<br><br>
**注**: OOBE 中に行われる Autopilot の自動暗号化を使用してデバイスが登録されている場合は、OS の既定値の代わりに使用されるポリシー ベースの設定を許可する Intune ポリシーが評価されるまで、トリガーされません。
 
Q: Intune ポリシーを適用した結果としてデバイスが暗号化されている場合、そのポリシーが削除されれば、デバイスの暗号は解除されますか?<br>
A: 暗号化関連のポリシーを削除しても、構成されたドライブの暗号は解除されません。
 
Q: Intune コンプライアンス ポリシーで、Bitlocker が有効になっているにもかかわらず有効になっていないと表示されるのはどうしてですか?<br>
A: Intune コンプライアンス ポリシーの「Bitlocker 有効」設定では、 Windows デバイス正常性構成証明 (DHA) のクライアントを利用します。 このクライアントは、ブート時のデバイスの状態のみ評価します。 そのため、Bitlocker 暗号化が完了してからデバイスが再起動されていない場合、DHA クライアント サービスでは Bitlocker をアクティブな状態として報告しません。
 
 