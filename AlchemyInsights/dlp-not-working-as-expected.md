---
title: DLP が期待どおりに機能していない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932627"
---
# <a name="dlp-not-working-as-expected"></a>DLP が期待どおりに機能していない

**重要**: 多くの SharePoint Online および OneDrive をご利用のお客様は、バックグラウンドで実行されるサービスに対してビジネスに不可欠なアプリケーションを実行します。 これには、コンテンツの移行、データ損失防止 (DLP)、およびバックアップ ソリューションが含まれます。 これらの前例のない時期に、リモート作業シナリオでこれまで以上にサービスに依存しているユーザーに対して、SharePoint Online および OneDrive サービスの可用性と信頼性を確保するための措置を講じています。

この目的をサポートするため、平日の昼間の時間帯に、バックグラウンド アプリ (移行、DLP、およびバックアップ ソリューション) の調整制限を強化しました。 これらのアプリのスループットは、これらの期間では非常に制限されています。 ただし、同地域の夕方および週末には、サービスはバックグラウンド アプリからの非常に大量のリクエストを処理する準備が整います。

 **DLP のセットアップ**

Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？ その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。
  
DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)の情報を使用します。
  
 **DLP ポリシーの検索基準**
  
Office 365 セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。
  
- **組み込みの機密情報の種類**

    組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」を参照してください。

- **カスタムの機密情報の種類**

    カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)」の記事を使用してください。

**DLP ポリシーをテストする**

組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。 詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)」をご覧ください。

 **レポート**
  
- [DLP レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。

- [インシデント レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。
