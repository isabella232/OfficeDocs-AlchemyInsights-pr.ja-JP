---
title: 自動分類が AIP クライアントで期待どおりに動作しない
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4373"
ms.openlocfilehash: 93d15b8b65fd52a567ecbb6e1f84363bf2b38946c105896b0b5ef41e49d16ea9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53979714"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a>自動分類が AIP クライアントで期待どおりに動作しない

自動分類が期待どおりに動作しない場合は、次の推奨ガイドラインを使用してください。

1. 自動ラベル付けに問題がある場合は、「[Azure Information Protection の自動分類および推奨分類の条件を構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)」および「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を確認してください。
2. 適切に構成されていないスコープ付きポリシーを使用しているかどうかを確認してください: 「[スコープ付きポリシーを使用して特定のユーザーの Azure Information Protection ポリシーを構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)」。
3. ラベル付きドキュメントを添付するときに Outlook で自動ラベル付けが機能しない場合は、`DRMEncryptProperty` が「[セキュリティの IRM レジストリ設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)」の説明に従って定義されていないことを確認してください。
4. Azure Information Protection ポリシーに[組み込み情報タイプ](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)を使用した場合は、コンテンツが予想される形式と一致していることを確認してください。
5. ラベルが [**自動**] または [**推奨**] 用に適切に構成されていることを確認します。 ([**自動**] ラベル付けはすべての Microsoft 365 アプリで使用できますが、[**推奨**] は Outlook を除くすべての Microsoft 365 アプリで使用できます。)
6. 以前に手動でラベルが付けられているか、以前に上位の分類で自動的にラベルが付けられているドキュメントと電子メールには自動分類を使用できません。  詳細については、「[自動ラベルと推奨ラベルが適用されるしくみ](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)」をご覧ください。
7. それでも問題が発生する場合は、Azure Information Protection クライアント ログを収集し、エクスポートしたログをサポート チケットに添付してください。Azure Information Protection ログをエクスポートするには、
    - Office ドキュメントを開くか、Outlook で新しいメールを作成します。
    - [**保護/感度** > **へルプとフィードバック**] をクリックします。
    - [**ログのエクスポート**] をクリックします。
    - ログを選択した場所に保存し、自分のサービス要求に添付します。

追加情報については、次を参照してください。

- [Azure Information Protection の自動分類および推奨分類の条件を構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [Azure Information Protection を使用する一般的なシナリオの使い方ガイド](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [Azure Information Protection のドキュメントを確認する](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection のサブスクリプションと機能を確認する](https://azure.microsoft.com/pricing/details/information-protection)
- [Azure Information Protection の要件](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection のクイック スタート チュートリアル](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [Azure Information Protection クライアントをダウンロードする](https://www.microsoft.com/download/details.aspx?id=53018)
