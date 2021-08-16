---
title: 最新の Azure のメールによる請求書
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
- "9003801"
- "6866"
ms.openlocfilehash: caf300873c3a9a97502819c7938ecc86491795d2fc7b6f022ead5d38ca965b8c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082839"
---
# <a name="email-invoicing-in-azure"></a>Azure のメールによる請求書

メールによる請求書の優先設定を更新するには、課金プロファイルや請求先アカウントで所有者または共同作成者の役割であることが必要です。 選択したら、所有者、共同作成者、閲覧者、および請求書管理者ロールを持つすべてのユーザーが、課金プロファイルでメールでの請求書を受け取ります。

1. [Azure portal](https://portal.azure.com/) にサインインします。
2. **コストの管理と課金** で検索します。
3. 左側の **[請求書]** を選択し、ページの上部にある **[メールの請求書]** を選びます。
4. 複数の課金プロファイルがある場合は、そのうちの 1 つを選択して **[オプトイン]** を選びます。

5. **[更新]** を選択します。
6. 複数の課金プロファイルがある場合は、そのうちの 1 つを選択して **[オプトイン]** を選びます。

他のユーザーに表示、ダウンロード、および請求書の支払いのアクセス許可を付与するには、MCA または MPA 課金プロファイルの請求書管理者ロールを割り当てる必要があります。 メールで請求書を受け取ることを選択した場合は、ユーザーもメールで請求書を受け取ります。

1. [Azure portal](https://portal.azure.com/) にサインインします。
2. **コストの管理と課金** で検索します。
3. 左側の [**課金プロファイル**] を選びます。 課金プロファイルの一覧で、請求書管理者ロールを割り当てる課金プロファイルを選びます。
4. 左側で **アクセス制御 (IAM)** を選択し、ページの上部にある [**追加**] を選びます。

[役割] ドロップダウン リストで、[**請求書管理者**] を選択します。 アクセス権を付与するユーザーのメール アドレスを入力します。 [**保存**] を選択して、ロールを割り当てます。
