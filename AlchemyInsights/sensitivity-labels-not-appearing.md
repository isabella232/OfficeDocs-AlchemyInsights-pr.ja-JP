---
title: 機密ラベルが表示されない
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 67719380aea0481f96c03fa591542e8e5a6e6993
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40048657"
---
# <a name="sensitivity-labels-not-appearing"></a>機密ラベルが表示されない

機密ラベルにより、機密コンテンツを分類して保護できます。 機密ラベルは、Microsoft 365 コンプライアンス センター、Microsoft 365 セキュリティ センター、または Office 365 セキュリティ/コンプライアンス センターの [分類] > [機密ラベル] で作成できます。 この機能の詳細については、「[機密ラベルの概要](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)」を参照してください。

機密ラベルが構成されているのに Office アプリでそれらが表示されない場合は、次の点を確認してください。

- 対象のユーザーとグループに機密ラベルが[「発行されている」](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)ことを確認します。

- ユーザーが機密ラベルをサポートするアプリを使用していることを確認します。[「ドキュメントの機密ラベル」](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)を参照してください。

- [「Azure Information Protection のラベルを移行する」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)場合は、[「こちら」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)に一覧表示されている考慮事項を留意してください。

- データ損失防止 (DLP) サポート: 現在、DLP ポリシーの条件として使い道があるのは保持ラベルのみです。  機密ラベルは DLP ポリシーではまだサポートされていませんが、サポートに向けて取り組んでいます。

- 機密ラベルの暗号化が有効になっている場合は、次のいずれかを行えます。
    - アクセス許可を今すぐ割り当てる
    - ユーザーがアクセス許可を割り当てる


潜在的な問題に関する詳細情報については、「[機密ラベルの既知の問題](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)」を参照してください。