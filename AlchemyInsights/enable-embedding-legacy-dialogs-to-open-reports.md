---
title: レポートを開くためにレガシ ダイアログの組み込みを有効にする
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002931"
- "5612"
ms.openlocfilehash: c8a5634d5d79cbd584284b675e5db4e448a0d157
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814269"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a>レポートを開くためにレガシ ダイアログの組み込みを有効にする

**現象**

ユーザーがレポートを開くことができない。 "問題が発生しました。 詳細については、技術的な詳細を確認してください。"

**原因**

"フォーム記述子が null であるか、定義されていません" というエラーが原因で、レポートを UCI に読み込むことができません。 UCI のレポートでは現在もレガシ ダイアログが必要であるため、顧客のシステムで *allowlegacydialogsembedding* が有効になっている必要があります。

**解決方法**

1. **[設定] > [管理] > [システム設定] > [全般] タブ** の順に移動します。

2. [統一インターフェイス ブラウザー クライアントに特定のレガシ ダイアログを組み込むことができるようにする] を [**はい**] に設定します。
