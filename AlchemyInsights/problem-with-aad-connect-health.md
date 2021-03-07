---
title: AAD Connect Health の問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/04/2021
ms.locfileid: "50484087"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="061f2-102">AAD Connect Health の問題</span><span class="sxs-lookup"><span data-stu-id="061f2-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="061f2-103">外科手術を行う権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="061f2-104">グローバル管理者は既定でアクセス権を持っています。</span><span class="sxs-lookup"><span data-stu-id="061f2-104">Global Admins have access by default.</span></span> <span data-ttu-id="061f2-105">さらに、[ロール ベースのアクセス制御](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)を使用して、登録権限を共同作成者に委任できます。</span><span class="sxs-lookup"><span data-stu-id="061f2-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="061f2-106">必要なエンドポイントが有効になっていて、ファイアウォールが原因でブロックされていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="061f2-107">詳細については、[要件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="061f2-108">ネットワーク レイヤーによる SSL 検査の対象となるアウトバウンド通信が原因で、登録が失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="061f2-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="061f2-109">Azure AD Connect Health の通知設定を確認したことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="061f2-110">設定を確認してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-110">Please review your setting.</span></span> <span data-ttu-id="061f2-111">この[ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)は、Azure AD Connect Health 通知の通知設定を構成する方法を理解するのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="061f2-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="061f2-112">AAD Connect Health 同期レポートとそのダウンロード方法の詳細については、「[オブジェクト レベルの同期レポート](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="061f2-113">AAD Connect Health アラートのトラブルシューティングを行うには、「[AAD Connect Health データの鮮度アラートのトラブルシューティング ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)」従ってください。よくある質問については、「[AAD Connect Health のインストールに関する一般的な質問](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="061f2-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
