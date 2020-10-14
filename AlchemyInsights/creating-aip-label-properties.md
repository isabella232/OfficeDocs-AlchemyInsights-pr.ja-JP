---
title: AIP ラベル ポリシーを作成する
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732180"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="b7508-102">AIP ラベル ポリシーを作成する</span><span class="sxs-lookup"><span data-stu-id="b7508-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="b7508-103">Azure Information Protection (AIP) のラベルは、組織が通常作成および格納している、最も低い分類の個人データから最も高い分類の高機密性のデータまで、組織が通常作成および保存するデータの全範囲で使用することができます。</span><span class="sxs-lookup"><span data-stu-id="b7508-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="b7508-104">Azure Information Protection ポリシーは、Azure Information Protection (AIP) のクラシック クライアントに適用されます。また、[AIP の統合されたラベル クライアント](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history) ではありません。</span><span class="sxs-lookup"><span data-stu-id="b7508-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="b7508-105">AIP ポリシーには、次のようなさまざまな要素を構成できます。</span><span class="sxs-lookup"><span data-stu-id="b7508-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="b7508-106">管理者またはユーザーがドキュメントとメールを分類および保護 (省略可能) することができるオプション</span><span class="sxs-lookup"><span data-stu-id="b7508-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="b7508-107">ユーザーが文書を保存してメールを送信するときに分類を強制するオプション</span><span class="sxs-lookup"><span data-stu-id="b7508-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="b7508-108">このオプションでは、メール メッセージの添付ファイルに基づいて自動的にラベルを付けることができます。</span><span class="sxs-lookup"><span data-stu-id="b7508-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="b7508-109">Office アプリケーションに情報保護バーを表示するかどうかを制御するオプション</span><span class="sxs-lookup"><span data-stu-id="b7508-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="b7508-110">Azure Information Protection ポリシーに関するその他のオプションおよび情報については、[「Azure Information Protection ポリシーの概要」](https://docs.microsoft.com/azure/information-protection/overview-policy)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7508-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="b7508-111">AIP ポリシーに関する他の役に立つリソースについては、次を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7508-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="b7508-112">チュートリアル: Azure Information Protection ポリシー設定を構成し、新しいラベルを作成する</span><span class="sxs-lookup"><span data-stu-id="b7508-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b7508-113">Azure Information Protection ポリシーを構成する</span><span class="sxs-lookup"><span data-stu-id="b7508-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="b7508-114">秘密度ラベルとそのポリシーを作成して構成する</span><span class="sxs-lookup"><span data-stu-id="b7508-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="b7508-115">Azure Information Protection を使用する一般的なシナリオの使い方ガイド</span><span class="sxs-lookup"><span data-stu-id="b7508-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="b7508-116">Azure Information Protection のドキュメントを確認する</span><span class="sxs-lookup"><span data-stu-id="b7508-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="b7508-117">Azure Information Protection の要件</span><span class="sxs-lookup"><span data-stu-id="b7508-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="b7508-118">Azure Information Protection のクイック スタート チュートリアル</span><span class="sxs-lookup"><span data-stu-id="b7508-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="b7508-119">Azure Information Protection クライアントをダウンロードする</span><span class="sxs-lookup"><span data-stu-id="b7508-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)