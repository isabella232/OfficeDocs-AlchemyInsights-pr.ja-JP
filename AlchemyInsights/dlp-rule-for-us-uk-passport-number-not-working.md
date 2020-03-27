---
title: US/UK パスポート番号の DLP ルールが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977111"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>DLP-US/英国のパスポート番号に関する問題

**重要**: これらの従来の状況では、sharepoint Online と OneDrive のサービスの可用性を確保するための手順を実行しています。詳細については、「 [Sharepoint online の一時的な機能の調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**米/英国のパスポート番号に関する DLP の問題**

O365 で DLP 機密情報の種類を使用しているときに、**米/英国のパスポート番号**が含まれているコンテンツの**データ損失防止 (DLP)** に関する問題が発生していますか。 その場合は、DLP ポリシーの評価時に必要な情報がコンテンツに含まれていることを確認してください。
  
たとえば、信頼レベルが75% で構成された**米/英国のパスポート番号**ポリシーの場合、次のものが評価され、ルールをトリガーするために検出される必要があります。
  
- **[書式:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 9 桁の数字

- **[パターン:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 9 桁の連続する数字

- **[チェックサム:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** いいえ、チェックサムはありません

- **[定義:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP ポリシーは、抽出した約 300 文字が次の条件に該当することを検出した場合に、75% の確証を持ってそれがこの種類の機密情報であると特定します。

  - 関数 Func_usa_uk_passport がパターンに一致するコンテンツを検出した。

  - Keyword_passport のキーワードを検出した。

    たとえば、次のサンプルは**米国/英国のパスポート番号**のポリシーに対してトリガーされます。米国のパスポート番号123456789

コンテンツに対して US/UK パスポート番号が検出されるために必要な情報の詳細については、この記事の「[US/UK パスポート番号に関する機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)」セクションを参照してください。
  
さまざまな組み込みの機密情報の種類を使用している場合は、「[機密情報の種類の検索基準](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)」の記事でその他の種類に必要なものを参照してください。
  