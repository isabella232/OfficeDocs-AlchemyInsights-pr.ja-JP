---
title: SharePoint および OneDrive における Office ファイルの秘密度ラベルの制限事項
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12451"
- "9000181"
ms.openlocfilehash: e2fc8fcf27eb916f64e4235cd116d9a7096e6078391e72363421ac3de721f5ee
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/11/2021
ms.locfileid: "57899769"
---
# <a name="limitations-for-sensitivity-labels-for-office-files-in-sharepoint-and-onedrive"></a>SharePoint および OneDrive における Office ファイルの秘密度ラベルの制限事項

SharePoint と OneDrive で Office ファイルの秘密度ラベルを有効にする場合は、次のような要件と制限事項に注意してください。

- ファイルに PowerQuery データ、カスタム アドインによって格納されたデータ、またはカスタム XML パーツが含まれている場合、SharePoint と OneDrive は Office デスクトップ アプリからラベル付けおよび暗号化された一部のファイルを処理できません。
- SharePoint と OneDrive は、Azure Information Protection (AIP) ラベルを使用して既に暗号化した既存のファイルに秘密度ラベルを自動的に適用することはしません。 暗号化されたファイルに秘密度ラベルを適用するには: 
    - AIP ラベルが移行され、Microsoft 365 コンプライアンス センターに発行されていることを確認します。
    - ラベル付けされたファイルをダウンロードし、元の SharePoint または OneDrive の場所にアップロードします。
- 暗号化されたドキュメントの場合、印刷はサポートされていません。

制限事項の追加情報については、「[SharePoint および OneDrive の Office ファイルの秘密度ラベルを有効にする](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-sharepoint-onedrive-files#limitations)」を参照してください。
