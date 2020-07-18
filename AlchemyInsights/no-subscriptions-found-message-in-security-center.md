---
title: セキュリティ センターにサブスクリプションが見つかりませんというメッセージ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 0bf6b247c71de5238a3b6f53cb6e782b06563415
ms.sourcegitcommit: 6cffc12f6f7e6e2efee19e05685f8ee10a823dde
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/17/2020
ms.locfileid: "45160515"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="bdc64-102">セキュリティ センターにサブスクリプションが見つかりませんというメッセージ</span><span class="sxs-lookup"><span data-stu-id="bdc64-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="bdc64-103">Microsoft Defender セキュリティ センターにアクセスしているときに「サブスクリプションが見つかりません」というメッセージが表示される場合は、ポータルへのユーザーのログインに使用される Azure Active Directory (AAD) に Microsoft Defender ATP ライセンスがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="bdc64-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="bdc64-104">Windows E5 ライセンスと Office E5 ライセンスは、別のライセンスです。</span><span class="sxs-lookup"><span data-stu-id="bdc64-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="bdc64-105">ライセンスを購入したが、この AAD インスタンスにプロビジョニングされていない場合は、サポート案件をオープンします。</span><span class="sxs-lookup"><span data-stu-id="bdc64-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="bdc64-106">次のいずれかがあります:</span><span class="sxs-lookup"><span data-stu-id="bdc64-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="bdc64-107">可能性のあるライセンスのプロビジョニングの問題。</span><span class="sxs-lookup"><span data-stu-id="bdc64-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="bdc64-108">ユーザーが、サービスへの認証に使用されたものとは異なる Microsoft AAD に誤ってライセンスをプロビジョニングしました。</span><span class="sxs-lookup"><span data-stu-id="bdc64-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>