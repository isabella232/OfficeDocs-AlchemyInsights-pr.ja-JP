---
title: DLP が期待どおりに機能していない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079707"
---
# <a name="dlp-not-working-as-expected"></a>DLP が期待どおりに機能していない

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

 **DLP のセットアップ**

Office 365 で **データ損失防止 (DLP)** が期待どおりに機能していないという問題が発生している場合は、**DLP ポリシー** が正しくセットアップされていて、評価されるときに **DLP ポリシー** で検索される内容が自分のデータに含まれていることを確認します。
  
DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)の情報を使用します。
  
 **DLP ポリシーの検索基準**
  
セキュリティ/コンプライアンス センターで **組み込みの機密情報の種類** を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。
  
- **組み込みの機密情報の種類**

    組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を参照してください。

- **カスタムの機密情報の種類**

    カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)」の記事を使用してください。

**DLP ポリシーをテストする**

組み込みやカスタムの機密情報の種類を使用してデータをテストするには、**[分類]** > **[機密情報の種類]** で **[テストの種類]** オプションを使用します。詳細については、「[カスタムの機密情報の種類をテストする](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)」を参照してください。

 **レポート**
  
- [DLP レポート](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。

- [インシデント レポート](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。
