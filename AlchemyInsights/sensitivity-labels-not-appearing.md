---
title: 機密ラベルが表示されない
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: admin
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1778"
- "9000181"
ms.openlocfilehash: 72dc88a55b55954f34c95fa5b5038f472261c5bb
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758448"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="e1b3d-102">機密ラベルが表示されない</span><span class="sxs-lookup"><span data-stu-id="e1b3d-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="e1b3d-103">機密ラベルにより、機密コンテンツを分類して保護できます。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="e1b3d-104">機密ラベルは、Microsoft 365 コンプライアンス センター、Microsoft 365 セキュリティ センター、または Microsoft 365 セキュリティ/コンプライアンス センターの [分類] > [機密ラベル] で作成できます。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-104">They can be created in the Microsoft 365 compliance center, Microsoft 365 security center, or Microsoft 365 security & Compliance Center under Classification > Sensitivity labels.</span></span> <span data-ttu-id="e1b3d-105">この機能の詳細については、「[機密ラベルの概要](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-105">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="e1b3d-106">機密ラベルが構成されているのに Office アプリでそれらが表示されない場合は、次の点を確認してください。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-106">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="e1b3d-107">対象のユーザーとグループに機密ラベルが[「発行されている」](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)ことを確認します。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-107">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="e1b3d-108">ユーザーが機密ラベルをサポートするアプリを使用していることを確認します。[「ドキュメントの機密ラベル」](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-108">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?#bkmk_whereavailable).</span></span>

- <span data-ttu-id="e1b3d-109">[「Azure Information Protection のラベルを移行する」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)場合は、[「こちら」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)に一覧表示されている考慮事項を留意してください。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-109">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="e1b3d-110">データ損失防止 (DLP) サポート: 現在、DLP ポリシーの条件として使い道があるのは保持ラベルのみです。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-110">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="e1b3d-111">機密ラベルは DLP ポリシーではまだサポートされていませんが、サポートに向けて取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-111">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

- <span data-ttu-id="e1b3d-112">機密ラベルの暗号化が有効になっている場合は、次のいずれかを行えます。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-112">When encryption is enabled on a sensitivity label, you can choose either to:</span></span>
    - <span data-ttu-id="e1b3d-113">アクセス許可を今すぐ割り当てる</span><span class="sxs-lookup"><span data-stu-id="e1b3d-113">Assign permissions now</span></span>
    - <span data-ttu-id="e1b3d-114">ユーザーがアクセス許可を割り当てる</span><span class="sxs-lookup"><span data-stu-id="e1b3d-114">Let users assign permissions</span></span>


<span data-ttu-id="e1b3d-115">潜在的な問題に関する詳細情報については、「[機密ラベルの既知の問題](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e1b3d-115">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc).</span></span>