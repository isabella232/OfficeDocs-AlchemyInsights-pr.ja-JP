---
title: 原価管理を有効にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/08/2020
ms.locfileid: "49680445"
---
# <a name="enable-cost-management"></a>原価管理を有効にする

**「組織のコストが無効になっています」の意味は何ですか?**

Enterprise Agreement (EA) または Microsoft Customer Agreement (MCA)のアカウントを使用している組織では、コスト情報と価格の情報へのアクセスを無効にすることができます。

Azure ポータルにログインした後は、課金 API を使用して、請求書 (オプトイン後) と使用状況の詳細をプログラムで取得できます。

**その他のユーザーに請求書へのアクセスを許可する方法**

1. Azure ポータルの **サブスクリプションのブレード** に移動します。
2. [**請求書**] を選択してから、次に [**請求書にアクセス**] を選択します。
3. アクセスをオンにして、変更を保存すると、サブスクリプション範囲内役割のユーザーは請求書をダウンロードできます。

> [!NOTE]
> アカウント管理者は、メールで請求書を送信するように設定することもできます。 詳細については、「[メールで請求書を取得する](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date??)」を参照してください。

**ユーザーを課金リーダーの役割に追加する方法**

1. Azure ポータルの **サブスクリプションのブレード** に移動します。
2. [**アクセス制御 (IAM)]** を選択し、[**追加**] をクリックします。
3. [**ロールの選択**] ページで、[**課金リーダー]** を選びます。
4. 招待するユーザーのメールアドレスを入力し、[ **OK**] をクリックして招待状を送信します。
5. 課金内容のリーダーとして招待メールに記載の手順に従ってログインします。 詳細については、「[課金へのアクセス許可を付与](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in) ] を参照してください。

**おすすめのドキュメント**

- [EA ポータルでの DA および AO の表示を有効にする](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [原価管理に含まれている原価](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [サポートされる Microsoft Azure の提供](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [原価分析のコストを確認する](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [課金情報にアクセス許可を付与する](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Microsoft 顧客契約へのアクセス許可の確認](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date??WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






