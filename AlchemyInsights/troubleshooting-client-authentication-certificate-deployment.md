---
title: クライアント認証証明書の展開のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: cecbd091447e63f2d5012ceaf96e050c92a171e6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658991"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>クライアント認証証明書の展開のトラブルシューティング

Intune の NDES/SCEP クライアント証明書プロファイルおよび PKCS/PFX クライアント証明書プロファイルは、一般的に Wi-Fi、VPN、メールなどのその他のプロファイル タイプと組み合わせて使用され、ユーザーが企業リソースに対して認証できるようにします。 これらのプロファイル タイプがクライアント証明書プロファイルにリンクされるタイミングは、そのプロファイルの正常な展開に依存します。

多くの場合、当初のインフラストラクチャのセットアップとそれに関連するクライアント証明書プロファイルの構成では、トラブルシューティングが必要です。 NDES コネクタを適切にセットアップするための詳しい手順および証明書の展開における問題を特定するためのトラブルシューティングのガイダンスについては、以下を参照してください。 

- [Configure infrastructure to support SCEP with Intune (Intune を使用してインフラストラクチャを構成して SCEP をサポートする)](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune (Microsoft Intune を使用した SCEP 証明書プロファイルのトラブルシューティングの概要)](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

参照されている PowerShell スクリプトを使用して、構成を確認します。 詳細については、「[Intune Certificate connector verification scripts (Intune 証明書コネクタ検証スクリプト)](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority)」を参照してください。

  
**その他の一般的な問題**

**Intune 証明書コネクタを NDES コネクタ サーバーにインストールしようとすると、"The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request. (証明書の要求のパスワードを確認できません。そのパスワードが既に使用されている可能性があります。この要求で送信するための新しいパスワードを取得してください。)" というメッセージが表示される。**  

このメッセージは、証明書コネクタのインストールを管理者として実行する必要があることを意味します。

一部の環境では、Intune 証明書が実行されるサーバーはプロキシ サーバーを使用して Intune に接続する必要があるため、証明書コネクタ はプロキシを使用する必要があります。 状況によっては、構成されたプロキシ設定が NDES コネクタによって無視される場合があり、また、LocalSystem のセキュリティ コンテキストでの実行中にプロキシ設定を構成する必要がある場合があります。 
 
この問題を解決するには、Internet Explorer を SYSTEM として実行し、IE でプロキシを構成します。 Intune コネクタ サービスの再起動後に、NDES コネクタが Intune に接続します。

**ユーザー デバイスが SCEP 証明書を NDES から受信しなくなった。**

NDES サーバーに発行され、NDES コネクタのインストール中に指定されたクライアント認証証明書の有効期限が切れているか欠落している可能性があります。 解決方法: 
 
1. NDES コネクタをアンインストールします。  
2. 次の詳細情報を使用して、新しいクライアント認証証明書またはサーバー認証証明書を要求します。 
 
    - サブジェクト名: CN=external fqdn  
    - サブジェクトの別名 (両方必要です): DNS=external fqdn、DNS=internal fqdn 
 
3. 新しい証明書を使用して NDES コネクタを再インストールします。