---
title: 準拠デバイスで条件付きアクセスによりブロックされる
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9835"
- "9003257"
ms.openlocfilehash: 240bd25f4d62505202c8cd7ceabe4c1cd3d5c0b5
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038259"
---
# <a name="im-getting-blocked-by-conditional-access-with-compliant-device"></a>準拠デバイスで条件付きアクセスによりブロックされる

**強くお勧めするツール**

- [デバイス登録トラブルシューティング ツール](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 最も一般的なデバイス登録の問題に関するトラブルシューティングに役立つ包括的なツールです。
- [テスト デバイス登録接続スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - デバイスがシステム アカウントでデバイス登録エンドポイントにアクセスできるようにするために使用されるツールです。
- [Azure AD デバイス クリーンアップ スクリプト](https://github.com/mzmaili/AzureADDeviceCleanup) - お使いの環境で古いデバイスを探して管理するために使用されるツールです。

準拠デバイスで条件付きアクセスが失敗する理由、または組織のリソースへのサインイン要求中にユーザーが 「**ここからアクセスすることはできません**」というメッセージを受信する場合の一般的な理由を次に示します。

1. **デバイスが MDM で要求されるデバイスの状態を満たしていない**。

デバイスが Intune などの承認済みの MDM プロバイダーに登録されており、*準拠デバイスとしてマークされている* ことを確認します。 Intune の詳細については、この[ドキュメント](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment)をご覧ください。 デバイスのコンプライアンスと Intune についてさらに理解するには、「[コンプライアンス ポリシーを使用して、Intune で管理するデバイスのルールを設定する](https://docs.microsoft.com/mem/intune/protect/device-compliance-get-started)」を参照してください。 Intune でのデバイスの登録で問題が発生する場合は、「[Microsoft へのデバイス登録のトラブルシューティング](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune)」からトラブルシューティングの詳細を参照してください。 Intune のサポートをさらに希望する場合は、サポート リクエストを作成します。 この操作を行うには、[[Intune のヘルプ とサポートのページ](https://endpoint.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/SupportMenu/helpSupport)] にアクセスします。

2. **デバイスが組織のネットワークに参加していません**:

組織のリソースにアクセスするには、デバイスを組織のネットワークに直接接続するか、仮想プライベート ネットワーク (VPN) を使用して接続し、オンプレミスまたは Azure Active Directory に参加する必要があります。 組織のネットワークに作業デバイスを参加させるには、「[作業デバイスを組織のネットワークに参加させる](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network)」を参照してください。 個人用/BYOD デバイスを登録するには、「[組織のネットワークに個人用デバイスを登録する](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network)」を参照してください。

- デバイスがネットワークに参加しているかどうかを検証するには、[ここ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-register-device-on-network#to-verify-that-youre-registered)から登録済みのデバイスの手順を実行するか、[ ここ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-join-device-on-network#to-make-sure-youre-joined)から作業デバイスの手順を実行します。 問題の範囲を組織のネットワーク接続に指定するには、以下のガイドラインに従ってください。

    1. 職場または学校のアカウント (alain@contoso.com など) を使用して Windows にサインインします。
    2. VPN または DirectAccess を使って組織のネットワークに接続します。
    3. 接続した後、**Windows ロゴ キー + L** を押してデバイスをロックします。
    4. 仕事用または学校用のアカウントを使用してデバイスのロックを解除し、問題のあるアプリまたはサービスにもう一度アクセスしてみます。

"**ここからアクセスすることはできません**" というエラー メッセージが再び表示される場合は、他の場所に問題がある可能性があります。

3. **オペレーティング システムはサポートされていません**:

次に記載するものを含む、サポートされているバージョンのオペレーティング システムを実行していることを確認してください。

- **Windows クライアント**: Windows 7 以降

- **Windows Server**: Windows Server 2008 R2 以降

- **macOS**: macOS X 以降

- **Android および iOS**: Android および iOS モバイル オペレーティング システムの最新バージョン

4. **Web ブラウザはサポートされていません**。

以下のサポートされているブラウザーを検索してください。 Windows 1703 以降のバージョンでの Chrome のサポートでは、Windows 10 アカウント拡張機能が必要です。 Microsoft Edge 85+ の場合、デバイスのコンプライアンス情報を適切に渡すには、ユーザーがサインインしている必要があります。 詳細については、[こちら](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)を参照してください。

- **Windows 10** Microsoft Edge、Internet Explorer、Chrome
- **Windows 8 / 8.1**: Internet Explorer、 Chrome
- **Windows 7**: Internet Explorer、 Chrome
- **iOS**: Microsoft Edge、Intune Managed Browser、Safari
- **Android**: **Microsoft Edge**: Intune Managed Browser、Chrome
- **Windows Phone**: Microsoft Edge、Internet Explorer
- **Windows Server 2019**: Microsoft Edge、Internet Explorer、Chrome
- **Windows Server 2016**: Internet Explorer
- **Windows Server 2012 R2**: Internet Explorer
- **Windows Server 2008 R2**: Internet Explorer
- **macOS**: Chrome、Safari

「**そこにはアクセスできません**」というメッセージとトラブルシューティングの手順の詳細については、[こちら](https://docs.microsoft.com/azure/active-directory/user-help/user-help-device-remediation)を参照してください。
