---
title: VPN に関連する問題
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
- "1545"
- "9000076"
ms.openlocfilehash: 1d9c34350d16d96329d1ed56666119dba0433c93ccb7547da5dba4894531e1b4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53970984"
---
# <a name="vpn-related-issues"></a>VPN に関連する問題

MDM クライアントの VPN 接続を正常に実装するには、VPN インフラストラクチャの要件を正しく反映する展開済みのプロファイルが存在している必要があります。 調査しているクライアント プラットフォームの適切な設定については、次を参照してください。 

[Windows 10 and Windows Holographic device settings to add VPN connections using Intune (Windows 10 および Windows Holographic デバイスを設定して Intune を使用した VPN 接続を追加する)](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Add VPN settings on iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイスに VPN 設定を追加する)](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Android device settings to configure VPN in Intune (Intune で VPN を構成するための Android デバイスの設定)](https://docs.microsoft.com/intune/vpn-settings-android)  
[Add VPN settings on macOS devices in Microsoft Intune (Microsoft Intune で macOS デバイスおよび iPadOS デバイスに VPN 設定を追加する)](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

VPN プロファイルで認証に基づく証明書が使用されている場合、VPN プロファイルにリンクされているルート証明書プロファイルとクライアント認証証明書プロファイルが正常に展開されていることを確認してください。

**一般的な問題**

**VPN プロファイルをデバイスに展開しました。正常に展開されたと Intune に表示されていますが、デバイスが VPN に接続されていません。**

正常な状態とは、Intune が構成通りにプロファイルを展開したという意味です。 ただし、これらの構成がお使いのネットワークや認証要件に適合していない可能性があります。 接続の試行の詳細については、(VPN サーバーと NPS/Radius サーバー上の) インフラストラクチャと認証サービスのログを確認します。 ログを収集して確認するには、ネットワーク インフラストラクチャ チームまたはサードパーティ VPN ベンダーと連携する必要がある場合があります。

**iOS 用のカスタム VPN を構成した際に、アプリ単位の VPN 機能が利用できません。**

Intune での iOS デバイス用のアプリ単位の VPN は現在、特定の一覧に含まれるプロバイダーとパートナーに対して提供されており、これらのプロバイダーとパートナーはまた、証明書の前提条件を満たしてからでないとアプリ単位の VPN を構成できません。 詳細については、「[Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune (Intune で iOS/iPadOS 用のアプリ単位の仮想プライベート ネットワーク (NPN) をセットアップする)](https://docs.microsoft.com/intune/vpn-setting-configure-per-app)」を参照してください。 

Intune の VPN のすべての接続タイプの詳細については、「[ (VPN サーバーに接続するための VPN プロファイルを Intune で作成する)](https://docs.microsoft.com/intune/vpn-settings-configure)」を参照してください。  

**構成済みのドメインにアクセスしたときに iOS のオンデマンド VPN がトリガーされない**

自動 VPN 設定をテストするには、次の値を設定します。

I want to do the following (次の操作を実行する): **Evaluate each connection attempt (それぞれの接続の試行を評価する)** 

Choose whether to connect (接続するかどうかの選択): **Connect if needed (必要な場合は接続する)**

When users access these domains (ユーザーがこれらのドメインにアクセスした場合): **target (ターゲット)** *domain name (ドメイン名)*

上記の構成が正常に動作しない場合は、次の要素を追加します。

When this URL is unreachable, force connect the VPN (この URL に接続できない場合は、VPN を強制接続する): **BADURL**