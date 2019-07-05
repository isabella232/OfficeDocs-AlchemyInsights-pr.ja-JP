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
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389618"
---
# <a name="dlp-not-working-as-expected"></a>DLP が期待どおりに機能していない

Office 365の**データ損失防止 (DLP)** で問題が発生していませんか？ その場合は、**DLPポリシー**が正しく設定されていること、およびデータに**DLPポリシー**が評価のさいに探しているものが含まれていることを確認してください。
  
 **DLP のセットアップ:**
  
DLP ポリシーによって、組織の機密情報を識別および保護することができます。DLP ポリシーをセットアップするには、[こちら](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)の情報を使用します。
  
 **DLP ポリシーの検索基準:**
  
Office 365 セキュリティ/コンプライアンス センターで**組み込みの機密情報の種類**を使用する場合、これらの機密の種類を検出するときに、DLP ポリシーでは特定のパターンと要素が検索されます。
  
- **組み込みの機密情報の種類:**

    組み込みの機密の種類の詳細および機密の種類を検出するときに DLP ポリシーで検索される内容については、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」を参照してください。

- **カスタムの機密情報の種類:**

    カスタムの機密情報の種類を作成する場合、カスタムの機密の種類の作成方法については、「[カスタムの機密情報の種類を作成する](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)」の記事を使用してください。

 **レポート:**
  
- [DLP レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)で機密データの分析情報を取得します。

- [インシデント レポート](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)でイベントの特定の詳細を確認します。
