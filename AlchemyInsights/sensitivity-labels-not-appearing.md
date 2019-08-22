---
title: 機密ラベルが表示されない
ms.author: stephow
author: stephow-MSFT
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
ms.openlocfilehash: be5fac4cf4f1516575b8310347dd1d1948010538
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36504540"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="07d92-102">機密ラベルが表示されない</span><span class="sxs-lookup"><span data-stu-id="07d92-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="07d92-103">機密ラベルを使用すると、機密コンテンツの分類と保護に役立ちます。</span><span class="sxs-lookup"><span data-stu-id="07d92-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="07d92-104">この機能の詳細については、「[機密ラベルの概要](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07d92-104">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="07d92-105">機密ラベルを構成したものの、Office アプリに表示されていない場合は、次の点を確認してください。</span><span class="sxs-lookup"><span data-stu-id="07d92-105">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="07d92-106">機密ラベルが必要なユーザーおよびグループに[公開](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)されていることを確認します。</span><span class="sxs-lookup"><span data-stu-id="07d92-106">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="07d92-107">ユーザーが機密ラベルをサポートするアプリを使用していることを確認します。[ドキュメントの「機密ラベル](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07d92-107">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="07d92-108">[Azure Information Protection のラベルを移行](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)する場合は、[ここ](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)に記載されている考慮事項に注意してください。</span><span class="sxs-lookup"><span data-stu-id="07d92-108">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="07d92-109">データ損失防止 (DLP) のサポート: 現在、DLP ポリシーの条件として使用できるのは、保持ラベルのみです。</span><span class="sxs-lookup"><span data-stu-id="07d92-109">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="07d92-110">DLP ポリシーでの機密ラベルのサポートは、まだ利用できませんが、作業中です。</span><span class="sxs-lookup"><span data-stu-id="07d92-110">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

<span data-ttu-id="07d92-111">考えられる問題の詳細については、「[既知の問題 (機密ラベル](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US))」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="07d92-111">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US).</span></span>