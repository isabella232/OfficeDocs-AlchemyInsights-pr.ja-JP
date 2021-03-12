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
ms.openlocfilehash: c3bf5dd9066685af2df7ba50f0eb3ba6e891c2a9
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708679"
---
# <a name="monitoring-conditional-access-for-exchange"></a>Exchange の条件付きアクセスを監視する

条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。

- そのデバイスが登録されていると推測される場合、ポータル サイト アプリに移動して、ポータル サイトに表示されていることを確認するようユーザーに勧めます。表示されない場合、ユーザーはそのデバイスを登録する必要があります。
- Azure portal で [Intune]、[デバイス ポリシー準拠] の順に選びます。 [監視] の下の、[デバイス準拠] をクリックします。 デバイス準拠レポートで、ユーザーのデバイスが準拠としてマークされていることを確認します。
- Azure portal で [Intune]、[デバイス ポリシー準拠] の順に選びます。 [管理] で [プロパティ] をクリックします。 コンプライアンス ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。 プロファイルが割り当てられていない場合、Intune はデバイスの準拠状況を確認することができません。
- ユーザーの条件付きアクセス割り当てを編集します。

1. Azure ポータルで、**[Intune]**  >  **[条件付きアクセス]**  >  **[ポリシー]** と移動します。
2. 一覧からポリシーを選択します。
3. [ユーザーとグループ] をクリックします。
4. 特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを [対象リスト] に追加します。 特定のユーザーに対して特定のポリシーを対象外とするには、それらのユーザーを [除外リスト] に追加します。

便利なリンク:

[デバイス コンプライアンスの概要](https://docs.microsoft.com/intune/device-compliance-get-started)

[CA のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-conditional-access)

[トラブルシューティング ポリシー](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-policies-in-microsoft-intune)

[Intune デバイス コンプライアンスの監視](https://docs.microsoft.com/intune/compliance-policy-monitor)

注: これらの手順は、Azure Active Directory 機能の条件付きアクセスに関するトラブルシューティングを行う場合にのみ役立ちます。 また、Exchange ポリシーを使用してメール アクセスをブロックしているデバイスを検疫することも可能です。 Exchange デバイス管理の詳細については、[こちら](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141) を参照してください。
