---
title: 9001220 高度な追及のカスタム検出
ms.author: dolmont
author: DulceMontemayor
manager: dansimp
ms.date: 09/25/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200"
- "9001220"
ms.assetid: ''
ms.openlocfilehash: 935508b3084aee0613d2bd1c2f26a437390f8640
ms.sourcegitcommit: fc62091696591175280c02c29876530d485c7871
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/26/2020
ms.locfileid: "48300133"
---
# <a name="advanced-hunting-custom-detections"></a><span data-ttu-id="5af20-102">高度な追及のカスタム検出</span><span class="sxs-lookup"><span data-stu-id="5af20-102">Advanced Hunting Custom detections</span></span>

<span data-ttu-id="5af20-103">高度な追及クエリに基づいてカスタム検出ルールを作成および管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="5af20-103">You can learn how to create and manage custom detections rules based on advanced hunting queries.</span></span> <span data-ttu-id="5af20-104">カスタム検出を使用すると、違反の疑いのあるアクティビティやデバイスの設定ミスなど、さまざまなイベントやシステム状態を事前に監視して対応できます。</span><span class="sxs-lookup"><span data-stu-id="5af20-104">With custom detections, you can proactively monitor for and respond to various events and system states, including suspected breach activity and misconfigured devices.</span></span> <span data-ttu-id="5af20-105">アラートと応答アクションを自動的にトリガーするカスタマイズ可能な検出ルールを使用してこれを行うことができます</span><span class="sxs-lookup"><span data-stu-id="5af20-105">You can do so with customizable detection rules that automatically trigger alerts and response actions</span></span>
  
<span data-ttu-id="5af20-106">Microsoft Defender ATP を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5af20-106">If you are using Microsoft Defender ATP, see the following topics for details:</span></span> 
- [<span data-ttu-id="5af20-107">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="5af20-107">Custom detections overview</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/overview-custom-detections)
- [<span data-ttu-id="5af20-108">検出ルールの作成</span><span class="sxs-lookup"><span data-stu-id="5af20-108">Create custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detection-rules)
- [<span data-ttu-id="5af20-109">検出ルールの表示と管理</span><span class="sxs-lookup"><span data-stu-id="5af20-109">View and manage custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detections-manage)

<span data-ttu-id="5af20-110">Microsoft Threat Protection を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="5af20-110">If you are using Microsoft Threat Protection, see the following topics for details:</span></span> 
- [<span data-ttu-id="5af20-111">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="5af20-111">Custom detections overview</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detections-overview)
- [<span data-ttu-id="5af20-112">カスタム検出ルールを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="5af20-112">Create and manage custom detections rules</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detection-rules)
