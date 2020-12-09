---
title: PRT 問題のトラブルシューティング
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/01/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000076"
- "7317"
ms.openlocfilehash: 8e654a38d720aa51daf21bf5c3fb0da8b9c3d8e7
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/04/2020
ms.locfileid: "49573963"
---
# <a name="troubleshoot-prt-issue"></a>PRT 問題のトラブルシューティング

デバイスの認証を完了するには、完全に登録され、良好な状態で、プライマリ更新トークン (PRT) を取得できる必要があります。

Hybrid Azure AD Join の登録プロセスを実行するには、デバイスが企業ネットワーク上にある必要があります。 VPN を経由して実行することもできますが、それにはいくつかの注意事項があります。 リモートワークのお客様のご要望にお応えして、Hybrid Azure AD Join の登録プロセスをトラブルシューティングするためのサポートを提供します。 ここでは、登録プロセスの裏側で何が起きているかの概要を示します。

**クラウド認証環境 (Azure AD パスワード ハッシュ同期またはパススルー認証の使用)**

この登録フローは "同期参加" とも呼ばれます。

1. Windows 10 は、ユーザーがデバイスにログオンするときに SCP レコードを検出します。
    1. まず、デバイスはクライアント側の SCP からの情報をレジストリ [HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD] に取得しようとします。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control)をご覧ください。
    2. 失敗した場合、デバイスは社内 Active Directory (AD) と通信し、サービス接続ポイント (SCP) からテナント情報を取得します。 SCP を検証するには、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-manual#configure-a-service-connection-point)を参照してください。 

> [!NOTE]
> AD で SCP を有効にし、クライアント側の SCP は最初の認証のときだけに使用することをおすすめします。

2. Windows 10 は Azure AD から認証を受けるために、システム コンテキストのもとで Azure AD との通信を試みます。 デバイスがシステム アカウントで Microsoft リソースにアクセスできるかどうかは、テスト デバイス登録接続スクリプトを使用して検証できます。

3. Windows 10 は自己署名証明書を生成し、社内 AD のコンピューター オブジェクトに格納します。 これにはドメイン コントローラーまでの照準線が必要です。

4. 証明書があるデバイス オブジェクトは、Azure AD Connect を経由して Azure AD に同期されます。 同期サイクルは既定で 30 分間隔ですが、Azure AD Connect の構成によって異なります。 詳細については、この[ドキュメント](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sync-configure-filtering#organizational-unitbased-filtering)を参照してください。

5. この時点で、当該のデバイスが Azure ポータルのデバイス ブレードに "保留中" の状態で表示されるようになります。

6. ユーザーが次回 Windows 10 にログインするときに、登録が完了します。 

> [!NOTE]
> デバイスが VPN 上にあり、ログオフとログインのプロセスがドメイン接続を終了させる場合、手動で登録を開始することができます。
 1. dsregcmd /join をローカルで管理者プロンプトに、または PSExec からリモートで PC に発行します。 例: PsExec -s \\win10client01 cmd、dsregcmd /join

 2. ハイブリッド参加の問題の詳細については、「[デバイスの問題のトラブルシューティング](https://techcommunity.microsoft.com/t5/azure-active-directory-identity/azure-ad-mailbag-frequent-questions-about-using-device-based/ba-p/1257344)」をご覧ください。
