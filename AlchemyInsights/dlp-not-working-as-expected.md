---
title: DLP が期待どおりに機能していない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: efb4a19f345fe6b8a1e8bb72abeba4a923c05777
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704418"
---
# <a name="dlp-not-working-as-expected"></a>DLP が期待どおりに機能していない

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

 **DLP のセットアップ**

Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？ その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。
  
DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)の情報を使用します。
  
 **DLP ポリシーの検索基準**
  
セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。
  
- **組み込みの機密情報の種類**

    組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」を参照してください。

- **カスタムの機密情報の種類**

    カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)」の記事を使用してください。

**DLP ポリシーをテストする**

組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。 詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)」をご覧ください。

 **レポート**
  
- [DLP レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。

- [インシデント レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。
