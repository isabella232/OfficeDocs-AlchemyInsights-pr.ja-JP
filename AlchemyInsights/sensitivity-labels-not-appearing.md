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
ms.openlocfilehash: 7336a6603b160a43b71e722487728df9af3e15b4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/28/2019
ms.locfileid: "35355738"
---
# <a name="sensitivity-labels-not-appearing"></a><span data-ttu-id="b13d3-102">機密ラベルが表示されない</span><span class="sxs-lookup"><span data-stu-id="b13d3-102">Sensitivity labels not appearing</span></span>

<span data-ttu-id="b13d3-103">機密ラベルにより、機密コンテンツを分類して保護できます。</span><span class="sxs-lookup"><span data-stu-id="b13d3-103">Sensitivity labels allow you to classify and help protect your sensitive content.</span></span> <span data-ttu-id="b13d3-104">この機能の詳細については、[「機密ラベルの概要」](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b13d3-104">To learn more about this feature, see [Overview of sensitivity labels](https://docs.microsoft.com/office365/securitycompliance/sensitivity-labels).</span></span>

<span data-ttu-id="b13d3-105">機密ラベルが構成されているのに Office アプリでそれらが表示されない場合は、次の点を確認してください。</span><span class="sxs-lookup"><span data-stu-id="b13d3-105">If you configured your sensitivity labels but they aren't appearing in the Office apps, check the following:</span></span>

- <span data-ttu-id="b13d3-106">対象のユーザーとグループに機密ラベルが[「発行されている」](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do)ことを確認します。</span><span class="sxs-lookup"><span data-stu-id="b13d3-106">Confirm that the sensitivity label has been [published](https://docs.microsoft.com/Office365/SecurityCompliance/sensitivity-labels#what-label-policies-can-do) to the users and groups that you want.</span></span>

- <span data-ttu-id="b13d3-107">ユーザーが機密ラベルをサポートするアプリを使用していることを確認します。[「ドキュメントの機密ラベル」](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b13d3-107">Confirm that the user is using an app that supports sensitivity labels - see [sensitivity labels in your document](https://support.office.com/article/apply-sensitivity-labels-to-your-documents-and-email-within-office-2f96e7cd-d5a4-403b-8bd7-4cc636bae0f9?ad=US&ui=en-US&rs=en-US#bkmk_whereavailable).</span></span>

- <span data-ttu-id="b13d3-108">[「Azure Information Protection のラベルを移行する」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)場合は、[「こちら」](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels)に一覧表示されている考慮事項を留意してください。</span><span class="sxs-lookup"><span data-stu-id="b13d3-108">If you're [migrating Azure Information Protection labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels), be aware of the considerations listed [here](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#considerations-for-unified-labels).</span></span>

- <span data-ttu-id="b13d3-109">データ損失防止 (DLP) サポート: 現在、DLP ポリシーの条件として使い道があるのは保持ラベルのみです。</span><span class="sxs-lookup"><span data-stu-id="b13d3-109">Data loss prevention (DLP) support: Currently, only retention labels can be used as a condition in DLP policies.</span></span>  <span data-ttu-id="b13d3-110">DLP ポリシーで機密ラベルをサポートすることは、今のところできませんが、それに向けて取り組んでいます。</span><span class="sxs-lookup"><span data-stu-id="b13d3-110">Support for sensitivity labels in a DLP policy is not available yet but we're working on it.</span></span>

<span data-ttu-id="b13d3-111">潜在的な問題に関する詳細情報については、[「機密ラベルの既知の問題」](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b13d3-111">For more information on possible issues, see [Known issues with sensitivity labels](https://support.office.com/article/known-issues-with-sensitivity-labels-in-office-b169d687-2bbd-4e21-a440-7da1b2743edc?ui=en-US&rs=en-US&ad=US).</span></span>