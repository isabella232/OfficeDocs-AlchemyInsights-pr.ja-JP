---
title: 自動分類が AIP クライアントで期待どおりに動作しない
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
- "4373"
ms.openlocfilehash: d7a2246d78cbd6c4ab40c2a4e5a21807933b619a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715206"
---
# <a name="automatic-classification-not-behaving-as-expected-with-the-aip-client"></a><span data-ttu-id="11232-102">自動分類が AIP クライアントで期待どおりに動作しない</span><span class="sxs-lookup"><span data-stu-id="11232-102">Automatic classification not behaving as expected with the AIP client</span></span>

<span data-ttu-id="11232-103">自動分類が期待どおりに動作しない場合は、次の推奨ガイドラインを使用してください。</span><span class="sxs-lookup"><span data-stu-id="11232-103">Automatic classification not behaving as expected, use the following recommended guidelines:</span></span>

1. <span data-ttu-id="11232-104">自動ラベル付けに問題がある場合は、「[Azure Information Protection の自動分類および推奨分類の条件を構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)」および「[機密情報の種類の検索基準](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)」を確認してください。</span><span class="sxs-lookup"><span data-stu-id="11232-104">If you are having issues with automatic labeling, see [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
2. <span data-ttu-id="11232-105">適切に構成されていないスコープ付きポリシーを使用しているかどうかを確認してください: 「[スコープ付きポリシーを使用して特定のユーザーの Azure Information Protection ポリシーを構成する方法](https://docs.microsoft.com/azure/information-protection/configure-policy-scope)」。</span><span class="sxs-lookup"><span data-stu-id="11232-105">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
3. <span data-ttu-id="11232-106">ラベル付きドキュメントを添付するときに Outlook で自動ラベル付けが機能しない場合は、`DRMEncryptProperty` が「[セキュリティの IRM レジストリ設定](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options)」の説明に従って定義されていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="11232-106">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that `DRMEncryptProperty` isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>
4. <span data-ttu-id="11232-107">Azure Information Protection ポリシーに[組み込み情報タイプ](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b)を使用した場合は、コンテンツが予想される形式と一致していることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="11232-107">If you used the [built-in information types](https://support.office.com/article/What-the-sensitive-information-types-look-for-fd505979-76be-4d9f-b459-abef3fc9e86b) for your Azure Information Protection policy, verify that your content matches the expected format.</span></span>
5. <span data-ttu-id="11232-108">ラベルが [**自動**] または [**推奨**] 用に適切に構成されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="11232-108">Verify that the label is appropriately configured for **Automatic** or **Recommended**.</span></span> <span data-ttu-id="11232-109">([**自動**] ラベル付けはすべての Microsoft 365 アプリで使用できますが、[**推奨**] は Outlook を除くすべての Microsoft 365 アプリで使用できます。)</span><span class="sxs-lookup"><span data-stu-id="11232-109">(**Automatic** labeling is available for all Microsoft 365 apps, whereas **Recommended** is available for all Microsoft 365 apps except for Outlook.)</span></span>
6. <span data-ttu-id="11232-110">以前に手動でラベルが付けられているか、以前に上位の分類で自動的にラベルが付けられているドキュメントと電子メールには自動分類を使用できません。</span><span class="sxs-lookup"><span data-stu-id="11232-110">You cannot use automatic classification for documents and emails that were previously manually labeled or previously automatically labeled with a higher classification.</span></span>  <span data-ttu-id="11232-111">詳細については、「[自動ラベルと推奨ラベルが適用されるしくみ](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="11232-111">For more information, see: [How automatic or recommended labels are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-classification#how-automatic-or-recommended-labels-are-applied).</span></span>
7. <span data-ttu-id="11232-112">それでも問題が発生する場合は、Azure Information Protection クライアント ログを収集し、エクスポートしたログを自分のサポート チケットに添付してください。</span><span class="sxs-lookup"><span data-stu-id="11232-112">If you are still experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to your support ticket.</span></span> <span data-ttu-id="11232-113">Azure Information Protection ログをエクスポートするには:</span><span class="sxs-lookup"><span data-stu-id="11232-113">To export Azure Information Protection logs:</span></span>
    - <span data-ttu-id="11232-114">Office ドキュメントを開くか、Outlook で新しいメールを作成します。</span><span class="sxs-lookup"><span data-stu-id="11232-114">Open an Office document or create a new email in Outlook.</span></span>
    - <span data-ttu-id="11232-115">[**保護/感度** > **へルプとフィードバック**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="11232-115">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
    - <span data-ttu-id="11232-116">[**ログのエクスポート**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="11232-116">Click **Export Logs**.</span></span>
    - <span data-ttu-id="11232-117">ログを選択した場所に保存し、自分のサービス要求に添付します。</span><span class="sxs-lookup"><span data-stu-id="11232-117">Save the logs to your choice of location, and attach them to your service request.</span></span>

<span data-ttu-id="11232-118">追加情報については、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="11232-118">For additional information, see:</span></span>

- [<span data-ttu-id="11232-119">Azure Information Protection の自動分類および推奨分類の条件を構成する方法</span><span class="sxs-lookup"><span data-stu-id="11232-119">How to configure conditions for automatic and recommended classification for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-classification)
- [<span data-ttu-id="11232-120">Azure Information Protection を使用する一般的なシナリオの使い方ガイド</span><span class="sxs-lookup"><span data-stu-id="11232-120">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)
- [<span data-ttu-id="11232-121">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="11232-121">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="11232-122">Azure Information Protection のサブスクリプションと機能を確認する</span><span class="sxs-lookup"><span data-stu-id="11232-122">Review Azure Information Protection subscriptions and features</span></span>](https://azure.microsoft.com/pricing/details/information-protection)
- [<span data-ttu-id="11232-123">Azure Information Protection の要件</span><span class="sxs-lookup"><span data-stu-id="11232-123">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="11232-124">Azure Information Protection のクイック スタート チュートリアル</span><span class="sxs-lookup"><span data-stu-id="11232-124">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)
- [<span data-ttu-id="11232-125">Azure Information Protection クライアントをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="11232-125">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
