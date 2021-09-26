---
title: 電子情報開示の推定値と実際の結果の違い
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13997"
- "3200003"
ms.openlocfilehash: e2a1f5ac688adc449286f920d4392adeb3fbd947
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506165"
---
# <a name="difference-in-ediscovery-estimates-and-actual-results"></a>電子情報開示の推定値と実際の結果の違い

推定された検索結果と電子情報開示検索でエクスポートされた実際の結果の間に違いが見られる場合、不一致の理由には次のようなものがあります。

- 推定および結果のエクスポートの時点以降に発生した変更。
- エクスポートに含まれるインデックスなしアイテム。
- エクスポート中に、検索が再実行され、実際のメッセージが Exchange データベースから取得されます。
- SharePoint と OneDrive のインデックスなしアイテムは、検索の見積りに含まれていません。

説明と不一致のその他の理由のリストについては、「[電子情報開示の推定された検索結果と実際の検索結果の違い](https://docs.microsoft.com/microsoft-365/compliance/differences-between-estimated-and-actual-ediscovery-search-results)」を参照してください。