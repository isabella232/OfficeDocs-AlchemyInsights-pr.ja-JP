---
title: ドメイン参加済みのデバイスで条件付きアクセスによりブロックされる
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: f0d092dfbc805b1e4fa7d26803227118b39ecacca9fa330bb5de8458d4aa0f57
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53950301"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>ドメイン参加済みのデバイスで条件付きアクセスによりブロックされる

**強くお勧めするツール**

[デバイス登録トラブルシューティング ツール](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - 最も一般的なデバイス登録の問題に関するトラブルシューティングに役立つツールです。

[テスト デバイス登録接続スクリプト](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - デバイスがシステム アカウントでデバイス登録エンドポイントにアクセスできるようにするのに役立つスクリプトです。

[Azure AD デバイス クリーンアップ スクリプト](https://github.com/mzmaili/AzureADDeviceCleanup) - お使いの環境で古いデバイスを探して管理できるようにするためのスクリプトです。

ドメインに参加しているデバイス (Hybrid Azure AD) が条件付きアクセスで失敗するおそれがある一般的な理由を以下に示します。

1. **デバイス上に Azure AD PRT がない。** - デバイスが Azure AD プライマリ更新トークン (PRT) を保持しているか確認する必要があります。PRT の詳細については、この [ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)を参照してください。

Azure AD PRT を保持しているか確認するには、デバイスで `dsregcmd/status` コマンドを実行し、“AzureAdPrt” が “YES” であるかを確認します。

"AzureAdPrt" が "NO" の場合は、次を確認してください。

- **AD FS でフェデレーション環境を構築しており、ユーザーの家庭のネットワークからは AD FS へアクセスできない場合**: この場合は、"usernamemixed" エンドポイントがエクストラネットからアクセス可能であることを確認します。 AD FS へのアクセスが VPN 越しである場合は、ユーザーが VPN に接続していることを確認し、デバイスに再ログインします。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)をご覧ください。

- **デバイスの TPM に問題があり、デバイスを認証できない場合**: "tpm.msc" を実行し、TPM の状態が "準備完了" かどうかを確認します。 それ以外の場合は、`dsregcmd/leave` を実行し、デバイスを Azure AD に再び参加させます。 その後、もう一度お試しください。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)をご覧ください。

- **サードパーティ ID プロバイダーを使用しているが、これが WS-Trust プロトコル プロバイダーをサポートしていない場合**。 ドキュメントに記載されているとおり、Hybrid Azure AD Join を使用したデバイスは、この場合は動作しません。 サポートが必要な場合は、ID プロバイダーにお問い合わせください。

2. **ユーザーが Windows 10 Accounts なしで Chrome ブラウザーを使用している**、または **Chrome 用の Office 拡張機能を AAD Join を使用したデバイスまたは Hybrid AAD Join を使用したデバイスで PRT を自動的に使用しない**: デバイスベースの条件付きアクセス ポリシーが失敗し、“未登録のデバイス” エラー メッセージが表示されます。 Chrome ブラウザーを正しく使用するには、SCCM または Intune 経由で "Windows 10 Accounts" または "ユーザーの Chrome ブラウザーに Office 拡張機能" をインストールする必要があります。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)をご覧ください。

拡張機能をリモートでプッシュできない場合は、上記の拡張機能のいずれかを手動でインストールし、デバイスベースの条件付きアクセスの背後にあるアプリケーションにアクセスするようにユーザーに通知します。詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)をご覧ください。

3. **デバイスは正しく Hybrid Azure AD Join を使用するようになったが、Azure AD Connect または Azure portal での変更の同期で誤って削除または無効化された**: この場合は、デバイスで "AzureAdJoined" と "PRT" の状態が有効と表示された場合でも、デバイス オブジェクトは完全に参加したデバイスとして認識されなくなります。

この問題を解決するには、影響を受けたデバイスで`dsregcmd/leave` を実行し、Azure AD にもう一度参加してください。詳細については、 [ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices).を参照してください。

> [!NOTE]
> Windows 10、1809 更新プログラムで VPN またはクラウド プロキシを使用しているデバイスで、"AzureAdPrt" の状態に関する問題、または SSO を使用するアプリの問題 (PRT があるにもかかわらず、Outlook がメールボックスに接続しない場合) が発生する場合は、このパッチ [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) または 4 月の累積更新プログラム [KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) を適用して、これらのマシンで PRT 障害が発生しないようにします。

















