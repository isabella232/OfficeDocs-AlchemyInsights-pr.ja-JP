---
title: 'AIP: 期待どおりに動作しないポリシー'
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
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821632"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="88574-102">AIP: 期待どおりに動作しないポリシー</span><span class="sxs-lookup"><span data-stu-id="88574-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="88574-103">Azure Information Protection: 期待どおりに動作しないポリシーについては、次のさまざまなポリシーの問題に関する推奨ガイドラインを参照してください。</span><span class="sxs-lookup"><span data-stu-id="88574-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="88574-104">視覚的なマーキングに問題がある場合は、「[視覚的なマーキングが適用されるタイミング](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="88574-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="88574-105">自動ラベル付けに問題がある場合は、「[Azure Information Protection の自動分類および推奨分類の条件を構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)」および「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="88574-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="88574-106">ネイティブ/Pfile 保護に問題がある場合は、「[ファイル API の構成](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="88574-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="88574-107">適切に構成されていないスコープ付きポリシーを使用しているかどうかを確認してください: 「[スコープ付きポリシーを使用して特定のユーザーの Azure Information Protection ポリシーを構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)」。</span><span class="sxs-lookup"><span data-stu-id="88574-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="88574-108">ラベル付きドキュメントを添付するときに Outlook で自動ラベル付けが機能しない場合は、DRMEncryptProperty が「[セキュリティの IRM レジストリ設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)」の説明に従って定義されていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="88574-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="88574-109">それでも問題が発生する場合は、Azure Information Protection クライアント ログを収集し、エクスポートしたログをこのチケットに添付してください。</span><span class="sxs-lookup"><span data-stu-id="88574-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="88574-110">Office ドキュメントを開くか、Outlook で新しいメールを作成します。</span><span class="sxs-lookup"><span data-stu-id="88574-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="88574-111">[**保護/感度** > **へルプとフィードバック**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="88574-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="88574-112">[**ログのエクスポート**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="88574-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="88574-113">ログを選択した場所に保存し、このサービス要求に添付します。</span><span class="sxs-lookup"><span data-stu-id="88574-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="88574-114">追加情報:</span><span class="sxs-lookup"><span data-stu-id="88574-114">Additional resources:</span></span>

- [<span data-ttu-id="88574-115">Azure Information Protection 用の視覚的なマーキングのラベルを構成する方法</span><span class="sxs-lookup"><span data-stu-id="88574-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="88574-116">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="88574-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="88574-117">Microsoft 365 アプリで秘密度ラベルを使用する</span><span class="sxs-lookup"><span data-stu-id="88574-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

