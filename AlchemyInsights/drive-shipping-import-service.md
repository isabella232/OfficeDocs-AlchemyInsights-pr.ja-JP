---
title: Microsoft 365 インポート サービスのドライブ配送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2021
ms.locfileid: "52732086"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a>Microsoft 365 インポート サービスのドライブ配送

ドライブ配送を使用するには、PST をハード ドライブにコピーしてから、ハード ドライブを Microsoft に配送します。

ジョブを開始するには:

1. Microsoft 365 コンプライアンス センターの **[情報ガバナンス]** で、**[インポート]** を選択します。

1. **[インポート ジョブの種類の選択]** を選択し、**[次へ]** を選択します。

1. このインポート オプションの手順を確認するには、**[Microsoft の物理的な場所のいずれかにハード ドライブを送付する]** を選択します。

覚えておきたい点がいくつかあります。

- PST ファイルを Microsoft 365 メールボックスにインポートするには、Exchange Online で Mailbox Import Export の役割が割り当てられている必要があります。
20 GB を超える PST の場合、パフォーマンスに影響する可能性があります。

- 2.5 インチのソリッドステート ドライブ (SSD) または 2.5 インチまたは 3.5 インチの SATA II/III 内部ハード ドライブのみがサポートされています。
PST ファイルを含むハード ドライブは、BitLocker で暗号化する必要があります。

- ドライブ送付で PST ファイルを Microsoft 365 メールボックスにインポートする費用は、データ 1 GB 当たり $2 USD です。

PST のインポートにドライブ配送方法を使用する際の詳細については、「[ドライブ配送を使用して組織の PST ファイルをインポートする](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)」を参照してください。