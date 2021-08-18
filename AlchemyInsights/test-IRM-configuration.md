---
title: 新しい OME 機能について IRM 構成をテストする
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12428"
- "9000078"
ms.openlocfilehash: d084caabfbcfdd92d6b90554c9e2bef5f571a0227827332a5fb3d710d7bc4836
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899701"
---
# <a name="test-irm-configuration-for-new-ome-capabilities"></a>新しい OME 機能について IRM 構成をテストする

Microsoft 365 テナントが新しい OME 機能を使用するように構成されていることを確認するには、[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online-powershell) に接続しているときに次のコマンドレットを実行します。


1. `Get-IRMConfiguration` を実行して、テナントの IRM 構成を確認します。 これらの値が **True** に設定されていることを確認してください。
    
    **InternalLicensingEnabled**
    
    **ExternalLicensingEnabled**
    
    **AzureRMSLicensingEnabled**

2. ドメイン、送信者アドレス、受信者を使用して、`Test-IRMConfiguration` を実行します。 テストに合格しない場合は、IRM 構成を調査してください。

IRM 構成を確認する方法の詳細については、「[Exchange Online PowerShell で新しい OME 構成を確認する](https://docs.microsoft.com/microsoft-365/compliance/set-up-new-message-encryption-capabilities#verify-new-ome-configuration-in-exchange-online-powershell)」を参照してください。