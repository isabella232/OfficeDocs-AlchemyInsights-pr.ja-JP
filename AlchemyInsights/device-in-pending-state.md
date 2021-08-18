---
title: 保留状態のデバイス
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
- "9003244"
- "7319"
ms.openlocfilehash: 7d8a55f8c9a9fc30c653152c2f1b185874cea3ee
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330377"
---
# <a name="device-in-pending-state"></a>保留状態のデバイス

**前提条件:**

1. 初めてデバイス登録を設定する場合は、[Azure Active Directory (Azure AD) でのデバイス管理の概要](https://docs.microsoft.com/azure/active-directory/devices/overview?WT.mc_id=Portal-Microsoft_Azure_Support)を確認してください。このガイドでは、デバイスを Azure AD の制御下に配置する方法について説明しています。
2. デバイスを Azure AD に直接登録し、それらを Intune に登録する場合は、[構成済み Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) があり、最初に[ライセンス](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support)が設定されていることを確認する必要があります。
3. Azure AD およびオンプレミス AD で操作を実行する権限があることを確認してください。 デバイス登録の設定を管理できるのは、Azure AD のグローバル管理者のみです。 さらに、オンプレミスの Active Directory で自動登録を設定する場合は、Active Directory と AD FS (該当する場合) の管理者である必要があります。

Hybrid Azure AD Join の登録プロセスを実行するには、デバイスが企業ネットワーク上にある必要があります。 VPN を経由して実行することもできますが、それにはいくつかの注意事項があります。 リモートワークのお客様のご要望にお応えして、Hybrid Azure AD Join の登録プロセスをトラブルシューティングするためのサポートを提供します。

**クラウド認証環境 (Azure AD パスワード ハッシュ同期またはパススルー認証の使用)**

この登録フローは "同期参加" とも呼ばれます。

次に、登録プロセス中に発生する現象の詳細を示します。

1. Windows 10 は、ユーザーがデバイスにログオンすると、サービス接続ポイント (SCP) レコードを検出します。

    1. まず、デバイスはクライアント側の SCP からの情報をレジストリ [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] に取得しようとします。 詳細については、「[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)」を参照してください。
    1. 失敗した場合、デバイスは社内 Active Directory と通信し、SCP からテナント情報を取得します。 SCP を検証するには、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)を参照してください。

    **注**: Active Directory で SCP を有効にし、クライアント側の SCP は最初の認証のときだけに使用することをお勧めします。

2. Windows 10 は Azure AD から認証を受けるために、システム コンテキストのもとで Azure AD との通信を試みます。

    デバイスがシステム アカウントで Microsoft リソースにアクセスできるかどうかは、[テスト デバイス登録接続スクリプト](https://gallery.technet.microsoft.com/Test-Device-Registration-3dc944c0)を使用して検証できます。

3. Windows 10 は自己署名証明書を生成し、社内 Active Directory のコンピューター オブジェクトに格納します。これにはドメイン コントローラーまでの照準線が必要です。

4. 証明書があるデバイス オブジェクトは、Azure AD Connect を経由して Azure AD に同期されます。 同期サイクルは既定で 30 分間隔ですが、Azure AD Connect の構成によって異なります。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)をご覧ください。

5. この時点で、当該のデバイスが Azure ポータルのデバイス ブレードに「**保留中**」の状態で表示されるようになります。

6. ユーザーが次回 Windows 10 にログインするときに、登録が完了します。

    **注**: デバイスが VPN 上にあり、ログオフとログインがドメイン接続を終了させる場合、手動で登録を開始することができます。 それには、次の手順を実行します。
    
    `dsregcmd /join` をローカルで管理者プロンプトに、または PSExec からリモートで PC に発行します。\
    例: `PsExec -s \\win10client01 cmd, dsregcmd /join`

Azure Active Directory デバイス登録に関する一般的な問題については、「[デバイスに関する FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq)」を参照してください。
