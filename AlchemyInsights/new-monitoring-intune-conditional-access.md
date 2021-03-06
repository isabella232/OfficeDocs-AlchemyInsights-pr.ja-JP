---
title: Intune 条件付きアクセスを監視
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004636"
- "8386"
ms.openlocfilehash: e2803a49aaf087ac55b1fd62056e2b0af3fcd919
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/03/2021
ms.locfileid: "50428388"
---
# <a name="monitor-intune-conditional-access"></a>Intune 条件付きアクセスを監視

条件付きアクセスで対象となるユーザーは、組織のアクセス要件を満たしていない場合には通知電子メールを受信します。この状態を解消するには、以下の 1 つ以上の解決策をお勧めします。

1. デバイス登録が済んでいると想定される場合は、Intune ポータル サイト アプリを使い、デバイスがポータル サイトに表示されているかどうかを確認することを、ユーザーに勧めてください。 もし表示されていない場合、ユーザーがデバイスを登録する必要があります。
1. Azure portal で **[Intune]** > **[デバイス ポリシー準拠]** の順に選びます。 
1. デバイスのポリシー準拠レポートを表示して、ユーザーのデバイスがポリシー準拠と示されているかどうか確認するには、**モニター** で **[デバイスのポリシー準拠]** をクリックします。
1. Azure portal で **[Intune]** > **[デバイス ポリシー準拠]** の順に選びます。 **[管理]** で **[プロパティ]** をクリックします。 コンプライアンス ポリシーの一覧で、ユーザーのデバイスにプロファイルが割り当てられていることを確認します。 プロファイルが割り当てられていない場合、Intune はデバイスの準拠状況を確認することができません。
1. ユーザーの条件付きアクセス割り当てを編集します。
1. Azure portal で、**Intune** > **条件付きアクセス** > **ポリシー** にアクセスし、一覧からポリシーを選択し、**ユーザーとグループ** をクリックします。
1. 特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを **[対象リスト]** に追加します。 特定のユーザーに対して特定のポリシーを対象とするには、それらのユーザーを **[除外リスト]** に追加します。

**便利なリンク:**

- [デバイス コンプライアンスの概要](https://docs.microsoft.com/intune/device-compliance-get-started)
- [CA のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-conditional-access)
- [トラブルシューティング ポリシー](https://docs.microsoft.com/intune/troubleshoot-policies-in-microsoft-intune)
- [Intune デバイス コンプライアンスの監視](https://docs.microsoft.com/intune/compliance-policy-monitor)

> [!NOTE]
> これらの手順は、Azure Active Directory 機能の条件付きアクセスに関するトラブルシューティングを行う場合にのみ役立ちます。 また、Exchange ポリシーを使用してメール アクセスをブロックしているデバイスを検疫することも可能です。 Exchange デバイス管理の詳細については、[**こちら**](https://docs.microsoft.com/previous-versions/office/exchange-server-2010/ff959225(v=exchg.141)) を参照してください。
