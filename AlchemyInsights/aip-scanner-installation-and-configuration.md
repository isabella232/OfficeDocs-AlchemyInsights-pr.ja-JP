---
title: 'AIP スキャナー: インストールと構成'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358754"
---
# <a name="aip-scanner-installation-and-configuration"></a>AIP スキャナー: インストールと構成

**AIP スキャナーをインストールするには、次の推奨ガイドラインに従ってください**。

1. アップグレード中で、クリーン インストールを実行しない場合は、[Azure Information Protection スキャナーのアップグレード](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)のガイドラインに従っていることを確認してください。また、統合ラベル付けクライアントのガイドラインについては、「[Azure Information Protectionスキャナーのアップグレード](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)」をご覧ください。
2. すべての [ファイアウォールおよびネットワークインフラストラクチャ設定要件](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)に準拠していることを確認します。
3. [ポリシーの設定を確認](https://docs.microsoft.com/azure/information-protection/configure-policy)し、自動ラベル付けまたは既定のラベルが設定されていることを確認してください。
4. [Azure Information Protectionクライアントでサポートされるファイルの種類](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)に記載されているように、関連するファイルの種類がラベル/保護用に構成されていることを確認してください。 また、既定の動作を変更する場合は、「[ファイルの既定の保護レベルを変更する](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)」のガイドラインに従ってください。
5. スキャナー サービスを実行するよう構成されているユーザー アカウントに、構成されているすべてのリポジトリへのアクセス許可があることを確認します。
6. 依然として問題が発生する場合は、スキャナー ログをエクスポートし、サポート チケットに追加してください。

**Azure Information Protection スキャナー ログをエクスポートする**

1. スキャナー サービスを実行しているユーザー コンテキスト下の %localappdata%\Microsoft\MSIP に移動します。
2. MSIP フォルダーのすべてのコンテンツを圧縮します。
3. ログを選択した場所に保存し、自分のサービス要求に添付します。
4. また、「[Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)」を使うこともできます。

**追加情報については、次を参照してください**。
- [ファイルを自動的に分類および保護するための Azure Information Protection スキャナーを展開する](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Set-AIPAuthentication の トークン パラメーターを指定して使用する](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [検出サイクルを実行して、スキャナーのレポートを表示する](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Azure Information Protection のドキュメントを確認する](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Azure Information Protection の要件](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Azure Information Protection クライアントをダウンロードする](https://www.microsoft.com/download/details.aspx?id=53018)
