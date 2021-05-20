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
ms.openlocfilehash: ea478cfbbbe96065608990770e0453d8f2613981
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543006"
---
# <a name="advanced-hunting-custom-detections"></a><span data-ttu-id="77210-102">高度な追及のカスタム検出</span><span class="sxs-lookup"><span data-stu-id="77210-102">Advanced Hunting Custom detections</span></span>

<span data-ttu-id="77210-103">高度な追及クエリに基づいてカスタム検出ルールを作成および管理する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="77210-103">You can learn how to create and manage custom detections rules based on advanced hunting queries.</span></span> <span data-ttu-id="77210-104">カスタム検出を使用すると、違反の疑いのあるアクティビティやデバイスの設定ミスなど、さまざまなイベントやシステム状態を事前に監視して対応できます。</span><span class="sxs-lookup"><span data-stu-id="77210-104">With custom detections, you can proactively monitor for and respond to various events and system states, including suspected breach activity and misconfigured devices.</span></span> <span data-ttu-id="77210-105">アラートと応答アクションを自動的にトリガーするカスタマイズ可能な検出ルールを使用してこれを行うことができます</span><span class="sxs-lookup"><span data-stu-id="77210-105">You can do so with customizable detection rules that automatically trigger alerts and response actions</span></span>
  
<span data-ttu-id="77210-106">Microsoft Defender ATP を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="77210-106">If you are using Microsoft Defender ATP, see the following topics for details:</span></span> 
- [<span data-ttu-id="77210-107">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="77210-107">Custom detections overview</span></span>](/windows/security/threat-protection/microsoft-defender-atp/overview-custom-detections)
- [<span data-ttu-id="77210-108">検出ルールの作成</span><span class="sxs-lookup"><span data-stu-id="77210-108">Create custom detection rules</span></span>](/windows/security/threat-protection/microsoft-defender-atp/custom-detection-rules)
- [<span data-ttu-id="77210-109">検出ルールの表示と管理</span><span class="sxs-lookup"><span data-stu-id="77210-109">View and manage custom detection rules</span></span>](/windows/security/threat-protection/microsoft-defender-atp/custom-detections-manage)

<span data-ttu-id="77210-110">Microsoft 365 Defender を使用している場合、詳細については次のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="77210-110">If you are using Microsoft 365 Defender, see the following topics for details:</span></span> 
- [<span data-ttu-id="77210-111">カスタム検出の概要</span><span class="sxs-lookup"><span data-stu-id="77210-111">Custom detections overview</span></span>](/microsoft-365/security/mtp/custom-detections-overview)
- [<span data-ttu-id="77210-112">カスタム検出ルールを作成および管理する</span><span class="sxs-lookup"><span data-stu-id="77210-112">Create and manage custom detections rules</span></span>](/microsoft-365/security/mtp/custom-detection-rules)
