---
title: Intune Wi-Fi プロファイル
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
- "1548"
- "9000076"
ms.openlocfilehash: 5e5258806c8a38965467a8878bc8ac922c2668f21abe3602f479dcdaff8c9b5b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028225"
---
# <a name="intune-wi-fi-profiles"></a>Intune Wi-Fi プロファイル

MDM クライアントの Wi-Fi 接続を正常に実装するには、Wi-Fi インフラストラクチャの要件を反映する正しく展開されたプロファイルが存在している必要があります。 調査しているクライアント プラットフォームの適切な設定を確認するには、次を参照してください。 

[Add Wi-Fi settings for devices running Android in Microsoft Intune (Android を実行するデバイス用に Microsoft Intune で Wi-Fi 設定を追加する)](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune (Microsoft Intune で、Android Enterprise 専用の完全に管理されたデバイスに Wi-Fi 設定を追加する)](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune (Microsoft Intune で iOS デバイスおよび iPadOS デバイス用の Wi-Fi 設定を追加する)](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Add Wi-Fi settings for Windows 10 and later devices in Intune (Intune で Windows 10 以降のデバイスに Wi-Fi 設定を追加する)](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Import Wi-Fi settings for Windows devices in Intune (Intune で Windows デバイス用 Wi-Fi 設定をインポートする)](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**一般的な問題**

**Wi-Fi プロファイルで指定されている展開済み証明書に依存する Wi-Fi プロファイルを展開しようとしていますが、構成プロファイルにエラー状態が表示されます。**

デバイスが証明書を受信したことを確認します。

1. Intune で、[**すべてのデバイス**] に移動し、[デバイス]、[**デバイスの構成**] の順に選択します。

2. すべての必要なプロファイルが表示されていて、状態が正常であることを確認します。

3. Android プロファイルの場合、証明書チェーンに中間証明書がある場合は、それらの中間証明書が Android デバイスに展開されていることを確認します。

    証明書の状態を確認するには、[**デバイスの構成**] > [**プロファイル**] > [**Android 中間証明書**] > [**プロパティ**] > [**信頼できる証明書**] の順に移動します。

エラーが引き続き表示される場合は、[手順とトラブルシューティング] セクションを参照してください。 詳細については、「[Overview for troubleshooting SCEP certificate profiles with Microsoft Intune (Microsoft Intune を使用した SCEP 証明書プロファイルのトラブルシューティングの概要)](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)」を参照してください。

**Wi-Fi プロファイルをデバイスに展開しました。正常に展開されたと Intune に表示されていますが、デバイスが Wi-Fi に接続されていません。**

正常な状態とは、Intune が構成通りにプロファイルを展開したという意味です。 ただし、これらの構成がお使いのネットワークや認証要件に適合していない可能性があります。 接続の試行の詳細については、(Wi-Fi アクセス ポイント コントローラーおよび NPS/Radius サーバー上の) インフラストラクチャと認証サービスのログを確認します。 ログを収集して確認するには、ネットワーク インフラストラクチャ チームまたはサードパーティ Wi-Fi ベンダーと連携する必要がある場合があります。