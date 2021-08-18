---
title: デバイス タグまたはグループの作成と管理
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
- "11446"
- "9003537"
ms.openlocfilehash: c06ed00d7cf4bcb23fdcee12f446953918075728
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325654"
---
# <a name="create-and-manage-device-tags-or-groups"></a>デバイス タグまたはグループの作成と管理

デバイスにタグを追加して、論理グループ アフィリエーションを作成します。 デバイス タグはネットワークの適切なマッピングをサポートし、さまざまなタグを添付してコンテキストをキャプチャし、インシデントの一部として動的リストを作成できるようにします。 タグは、デバイス リスト ビューでフィルターとして使用したり、デバイスをグループ化するために使用できます。 デバイスのグループ化の詳細については、「[デバイス タグの作成と管理](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)」を参照してください。

次の方法でデバイスにタグを追加できます。

- ポータルを使用する

- レジストリ キー値を設定する
 
**注:** タグがデバイスに追加されてから、デバイス リストおよびデバイス ページにタグが表示されるまでには、遅延が発生する可能性があります。

API を使用してデバイス タグを追加するには、「[デバイス タグ API の追加または削除](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)」を参照してください。

## <a name="add-and-manage-device-tags-using-the-portal"></a>ポータルを使用してデバイス タグを追加および管理する

1. タグを管理するデバイスを選択します。 次のいずれかのビューからデバイスを選択または検索できます。

    - **セキュリティ運用ダッシュボード** [アクティブなアラートがある上位デバイス] セクションからデバイス名を選択します。
    - **アラート キュー** - アラート キューからデバイス アイコンの横にあるデバイス名を選択します。
    - **デバイス リスト** - デバイスのリストからデバイス名を選択します。
    - **検索ボックス** - ドロップダウン メニューから [デバイス] を選択し、デバイス名を入力します。

    ファイル ビューと IP ビューからアラート ページにアクセスすることもできます。

1. [応答] アクションの行から **[タグの管理]** を選択します。

1. 入力してタグを検索または作成します。

タグがデバイス ビューに追加され、デバイス リスト ビューに反映されます。 その後、[タグ] フィルターを使用して、関連するデバイスのリストを表示できます。

詳細については、「[デバイス タグの作成と管理](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/machine-tags)」を参照してください。