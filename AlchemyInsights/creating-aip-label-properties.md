---
title: AIP ラベルポリシーの作成
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569874"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="2d4a3-102">AIP ラベルポリシーの作成</span><span class="sxs-lookup"><span data-stu-id="2d4a3-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="2d4a3-103">Azure Information Protection (AIP) ラベルは、組織が通常、個人データの最も低い分類から非常に機密性の高いデータを分類するために作成および格納するあらゆるデータの範囲で使用できます。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="2d4a3-104">Azure Information Protection ポリシーは、Azure Information Protection (AIP) の従来のクライアントに適用され、 [AIP の統合ラベルクライアント](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history)には適用されません。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="2d4a3-105">AIP ポリシーでは、次のようなオプションを含む複数の要素を構成できます。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="2d4a3-106">管理者またはユーザーによるドキュメントおよび電子メールの分類と保護 (オプション) を許可するラベルのオプション</span><span class="sxs-lookup"><span data-stu-id="2d4a3-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="2d4a3-107">ユーザーがドキュメントを保存して電子メールを送信するときに分類を適用するオプション</span><span class="sxs-lookup"><span data-stu-id="2d4a3-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="2d4a3-108">電子メールメッセージの添付ファイルに基づいて、自動的にラベルを付けるオプション。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="2d4a3-109">Office アプリケーションで情報保護バーを表示するかどうかを制御するオプション</span><span class="sxs-lookup"><span data-stu-id="2d4a3-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="2d4a3-110">Azure Information Protection ポリシーに関するその他のオプションと情報については、「 [Azure Information protection ポリシーの概要](https://docs.microsoft.com/azure/information-protection/overview-policy)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="2d4a3-111">AIP ポリシーに関するその他の参考資料については、以下を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d4a3-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="2d4a3-112">チュートリアル: Azure Information Protection ポリシーの設定を構成し、新しいラベルを作成する</span><span class="sxs-lookup"><span data-stu-id="2d4a3-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="2d4a3-113">Azure Information Protection ポリシーを構成する</span><span class="sxs-lookup"><span data-stu-id="2d4a3-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="2d4a3-114">秘密度ラベルとそのポリシーを作成して構成する</span><span class="sxs-lookup"><span data-stu-id="2d4a3-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="2d4a3-115">Azure Information Protection を使用する一般的なシナリオの使い方ガイド</span><span class="sxs-lookup"><span data-stu-id="2d4a3-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="2d4a3-116">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="2d4a3-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="2d4a3-117">Azure Information Protection の要件</span><span class="sxs-lookup"><span data-stu-id="2d4a3-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="2d4a3-118">Azure Information Protection のクイック スタート チュートリアル</span><span class="sxs-lookup"><span data-stu-id="2d4a3-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="2d4a3-119">Azure Information Protection クライアントをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="2d4a3-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)