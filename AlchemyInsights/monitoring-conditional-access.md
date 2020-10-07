---
title: 条件付きアクセスを監視する
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003769"
- "6702"
ms.openlocfilehash: 0687875a3714067e774872d02630564858d71d1b
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366433"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange の条件付きアクセスを監視する

条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。

- そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。
- Azure portal で、[Intune > デバイスコンプライアンス] に移動します。[モニター] の [デバイスのコンプライアンス] をクリックします。デバイスコンプライアンスレポートを表示して、ユーザーのデバイスが準拠しているとしてマークされていることを確認します。
- Azure portal で、[Intune > デバイスコンプライアンス] に移動します。[管理] で、[ポリシー] をクリックします。コンプライアンスポリシーの一覧で、プロファイルがユーザーのデバイスに割り当てられていることを確認します。プロファイルが割り当てられていない場合、Intune はデバイスのコンプライアンスの状態を確認できません。
- ユーザーの条件付きアクセス割り当てを編集します。

1. Azure portal で、[ **Intune**  >  **条件付きアクセス**  >  **ポリシー**] に移動します。
2. リストからポリシーを選択します。
3. [ユーザーとグループ] をクリックします。
4. 特定のユーザーに対して特定のポリシーを対象とするには、[必要] リストに追加します。対象ポリシーから特定のユーザーを除外するには、[必要なし] リストに追加します。

便利なリンク:

[デバイス コンプライアンスの概要](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[トラブルシューティング ポリシー](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)

[Intune デバイスコンプライアンスの監視](https://docs.microsoft.com/intune/compliance-policy-monitor)

注: これらの手順は、Azure Active Directory 機能の条件付きアクセスのトラブルシューティングにのみ役立ちます。 Exchange ポリシーを使用して、電子メールへのアクセスをブロックするデバイスを検疫することもできます。 Exchange デバイス管理の詳細については、 [こちら](<https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141>)を参照してください。
