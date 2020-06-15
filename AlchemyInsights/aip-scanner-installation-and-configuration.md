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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="8f6eb-102">AIP スキャナー: インストールと構成</span><span class="sxs-lookup"><span data-stu-id="8f6eb-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="8f6eb-103">**AIP スキャナーをインストールするには、次の推奨ガイドラインに従ってください**。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="8f6eb-104">アップグレード中で、クリーン インストールを実行しない場合は、[Azure Information Protection スキャナーのアップグレード](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner)のガイドラインに従っていることを確認してください。また、統合ラベル付けクライアントのガイドラインについては、「[Azure Information Protectionスキャナーのアップグレード](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="8f6eb-105">すべての [ファイアウォールおよびネットワークインフラストラクチャ設定要件](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)に準拠していることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="8f6eb-106">[ポリシーの設定を確認](https://docs.microsoft.com/azure/information-protection/configure-policy)し、自動ラベル付けまたは既定のラベルが設定されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="8f6eb-107">[Azure Information Protectionクライアントでサポートされるファイルの種類](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection)に記載されているように、関連するファイルの種類がラベル/保護用に構成されていることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="8f6eb-108">また、既定の動作を変更する場合は、「[ファイルの既定の保護レベルを変更する](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files)」のガイドラインに従ってください。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="8f6eb-109">スキャナー サービスを実行するよう構成されているユーザー アカウントに、構成されているすべてのリポジトリへのアクセス許可があることを確認します。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="8f6eb-110">依然として問題が発生する場合は、スキャナー ログをエクスポートし、サポート チケットに追加してください。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="8f6eb-111">**Azure Information Protection スキャナー ログをエクスポートする**</span><span class="sxs-lookup"><span data-stu-id="8f6eb-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="8f6eb-112">スキャナー サービスを実行しているユーザー コンテキスト下の %localappdata%\Microsoft\MSIP に移動します。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="8f6eb-113">MSIP フォルダーのすべてのコンテンツを圧縮します。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="8f6eb-114">ログを選択した場所に保存し、自分のサービス要求に添付します。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="8f6eb-115">また、「[Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)」を使うこともできます。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="8f6eb-116">**追加情報については、次を参照してください**。</span><span class="sxs-lookup"><span data-stu-id="8f6eb-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="8f6eb-117">ファイルを自動的に分類および保護するための Azure Information Protection スキャナーを展開する</span><span class="sxs-lookup"><span data-stu-id="8f6eb-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="8f6eb-118">Set-AIPAuthentication の トークン パラメーターを指定して使用する</span><span class="sxs-lookup"><span data-stu-id="8f6eb-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="8f6eb-119">検出サイクルを実行して、スキャナーのレポートを表示する</span><span class="sxs-lookup"><span data-stu-id="8f6eb-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="8f6eb-120">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="8f6eb-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="8f6eb-121">Azure Information Protection の要件</span><span class="sxs-lookup"><span data-stu-id="8f6eb-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="8f6eb-122">Azure Information Protection クライアントをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="8f6eb-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
