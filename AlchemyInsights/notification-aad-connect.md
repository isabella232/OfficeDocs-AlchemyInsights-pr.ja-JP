---
title: AAD Connect の通知
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2021
ms.locfileid: "51038274"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="a2d50-102">AAD Connect の通知</span><span class="sxs-lookup"><span data-stu-id="a2d50-102">Notification AAD Connect</span></span>

- <span data-ttu-id="a2d50-103">外科手術を行う権限があることを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="a2d50-104">グローバル管理者は既定でアクセス権を持っています。</span><span class="sxs-lookup"><span data-stu-id="a2d50-104">Global Admins have access by default.</span></span> <span data-ttu-id="a2d50-105">さらに、[ロール ベースのアクセス制御](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations)を使用して、登録権限を共同作成者に委任できます。</span><span class="sxs-lookup"><span data-stu-id="a2d50-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="a2d50-106">必要なエンドポイントが有効になっていて、ファイアウォールが原因でブロックされていないことを確認してください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="a2d50-107">詳細については、[要件](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="a2d50-108">ネットワーク レイヤーによる SSL 検査の対象となるアウトバウンド通信が原因で、登録が失敗する可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a2d50-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="a2d50-109">Azure AD Connect Health の通知設定を確認して、自分の設定をレビューしてください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="a2d50-110">Azure AD Connect Health 通知の通知設定を構成する方法を理解するには、この[ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)が役立ちます。</span><span class="sxs-lookup"><span data-stu-id="a2d50-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="a2d50-111">AAD Connect Health 同期レポートとそのダウンロード方法の詳細については、「[オブジェクト レベルの同期レポート](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="a2d50-112">AAD Connect Health アラートのトラブルシューティングを行うには、「[AAD Connect Health データの鮮度アラートのトラブルシューティング ガイド](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness)」に従ってください。よくある質問については、「[AAD Connect Health のインストールに関する一般的な質問](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2d50-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
