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
ms.openlocfilehash: 40351bd7852b69e0ff2ae6f630749ecbc1e0f13b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801520"
---
# <a name="advanced-hunting-custom-detections"></a><span data-ttu-id="ade9f-102">高度な追及のカスタム検出</span><span class="sxs-lookup"><span data-stu-id="ade9f-102">Advanced Hunting Custom detections</span></span>

<span data-ttu-id="ade9f-103">高度な追及クエリに基づいてカスタム検出ルールを作成および管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="ade9f-103">You can learn how to create and manage custom detections rules based on advanced hunting queries.</span></span> <span data-ttu-id="ade9f-104">カスタム検出を使用すると、違反の疑いのあるアクティビティやデバイスの設定ミスなど、さまざまなイベントやシステム状態を事前に監視して対応できます。</span><span class="sxs-lookup"><span data-stu-id="ade9f-104">With custom detections, you can proactively monitor for and respond to various events and system states, including suspected breach activity and misconfigured devices.</span></span> <span data-ttu-id="ade9f-105">アラートと応答アクションを自動的にトリガーするカスタマイズ可能な検出ルールを使用してこれを行うことができます</span><span class="sxs-lookup"><span data-stu-id="ade9f-105">You can do so with customizable detection rules that automatically trigger alerts and response actions</span></span>
  
<span data-ttu-id="ade9f-106">Microsoft Defender ATP を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ade9f-106">If you are using Microsoft Defender ATP, see the following topics for details:</span></span> 
- [<span data-ttu-id="ade9f-107">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="ade9f-107">Custom detections overview</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/overview-custom-detections)
- [<span data-ttu-id="ade9f-108">検出ルールの作成</span><span class="sxs-lookup"><span data-stu-id="ade9f-108">Create custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detection-rules)
- [<span data-ttu-id="ade9f-109">検出ルールの表示と管理</span><span class="sxs-lookup"><span data-stu-id="ade9f-109">View and manage custom detection rules</span></span>](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/custom-detections-manage)

<span data-ttu-id="ade9f-110">Microsoft 365 Defender を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="ade9f-110">If you are using Microsoft 365 Defender, see the following topics for details:</span></span> 
- [<span data-ttu-id="ade9f-111">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="ade9f-111">Custom detections overview</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detections-overview)
- [<span data-ttu-id="ade9f-112">カスタム検出ルールを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="ade9f-112">Create and manage custom detections rules</span></span>](https://docs.microsoft.com/microsoft-365/security/mtp/custom-detection-rules)
