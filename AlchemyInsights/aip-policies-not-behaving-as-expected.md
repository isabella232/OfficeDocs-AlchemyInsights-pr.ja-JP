---
title: 'AIP: 期待どおりに動作しないポリシー'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 0dfaae776ec551fe12919e8a8e69f2e7a58d67d0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663194"
---
# <a name="aip-policies-not-behaving-as-expected"></a>AIP: 期待どおりに動作しないポリシー

Azure Information Protection: 期待どおりに動作しないポリシーについては、次のさまざまなポリシーの問題に関する推奨ガイドラインを参照してください。

1. 視覚的なマーキングに問題がある場合は、「[視覚的なマーキングが適用されるタイミング](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)」を確認してください。
2. 自動ラベル付けに問題がある場合は、「[Azure Information Protection の自動分類および推奨分類の条件を構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)」および「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を確認してください。
3. ネイティブ/Pfile 保護に問題がある場合は、「[ファイル API の構成](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)」を確認してください。
4. 適切に構成されていないスコープ付きポリシーを使用しているかどうかを確認してください: 「[スコープ付きポリシーを使用して特定のユーザーの Azure Information Protection ポリシーを構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)」。
5. ラベル付きドキュメントを添付するときに Outlook で自動ラベル付けが機能しない場合は、DRMEncryptProperty が「[セキュリティの IRM レジストリ設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)」の説明に従って定義されていないことを確認してください。

それでも問題が発生する場合は、Azure Information Protection クライアント ログを収集し、エクスポートしたログをこのチケットに添付してください。

1. Office ドキュメントを開くか、Outlook で新しいメールを作成します。
2. [**保護/感度** > **へルプとフィードバック**] をクリックします。
3. [**ログのエクスポート**] をクリックします。
4. ログを選択した場所に保存し、このサービス要求に添付します。

追加情報:

- [Azure Information Protection 用の視覚的なマーキングのラベルを構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [Azure Information Protection のドキュメントを確認する](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Microsoft 365 アプリで秘密度ラベルを使用する](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

