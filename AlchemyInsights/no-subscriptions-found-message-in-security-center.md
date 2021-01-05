---
title: セキュリティ センターにサブスクリプションが見つかりませんというメッセージ
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/15/2020
ms.locfileid: "47772609"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="7d64d-102">セキュリティ センターにサブスクリプションが見つかりませんというメッセージ</span><span class="sxs-lookup"><span data-stu-id="7d64d-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="7d64d-103">Microsoft Defender セキュリティ センターにアクセスしているときに「サブスクリプションが見つかりません」というメッセージが表示される場合は、ポータルへのユーザーのログインに使用される Azure Active Directory (AAD) に Microsoft Defender ATP ライセンスがないことを意味します。</span><span class="sxs-lookup"><span data-stu-id="7d64d-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="7d64d-104">Windows E5 ライセンスと Office E5 ライセンスは、別のライセンスです。</span><span class="sxs-lookup"><span data-stu-id="7d64d-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="7d64d-105">ライセンスを購入したが、この AAD インスタンスにプロビジョニングされていない場合は、サポート案件をオープンします。</span><span class="sxs-lookup"><span data-stu-id="7d64d-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="7d64d-106">次のいずれかがあります:</span><span class="sxs-lookup"><span data-stu-id="7d64d-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="7d64d-107">可能性のあるライセンスのプロビジョニングの問題。</span><span class="sxs-lookup"><span data-stu-id="7d64d-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="7d64d-108">ユーザーが、サービスへの認証に使用されたものとは異なる Microsoft AAD に誤ってライセンスをプロビジョニングしました。</span><span class="sxs-lookup"><span data-stu-id="7d64d-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>