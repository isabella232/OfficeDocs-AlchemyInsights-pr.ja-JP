---
title: Yammer の ID について
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: f417117acac4c3040932fc0a35e5d0b1c3709cd5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664175"
---
# <a name="about-identity-in-yammer"></a>Yammer の ID について

ID 関連の問題を回避するために、すべてのネットワークで次の手順を実行することをお勧めします:

1. Azure AD のユーザーに Microsoft 365 アカウントをプロビジョニングした後に Office 365 ID を適用して、すべてのユーザーが主要な Microsoft 365 アカウントを使用してサインインするようにします。 詳しくは、[「Yammer ユーザーに Office 365 ID を適用する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity) を参照してください。
2. 複数の Yammer ネットワークを統合します。 従来の Yammer 構成では、1 つのテナントに複数の Yammer ネットワークを接続できます。 詳しくは、[「ネットワークの移行 - 複数の Yammer ネットワークを統合する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) を参照してください。
3. 必要に応じて、ユーザーにライセンスがない場合に Yammer からユーザーをブロックするために、Yammer にライセンスを適用します。 詳しくは、[「Office 365 で Yammer ユーザー ライセンスを管理する」](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365) を参照してください。
4. 最後に、以前の Yammer ネットワークのユーザー リストを監査し、従来のユーザーを一時停止します。 削除は元に戻せないため、ユーザーを削除するのではなく、一時停止 （非アクティブ化） することをお勧めします。 詳しくは、[「Office 365 に接続されているネットワークで Yammer ユーザーを監査する」](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) と [「ユーザーを削除する」](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users) を参照してください。

これらの手順を使用して Yammer を構成すると、Microsoft 365 のネイティブ モードで Yammer ネットワークを構成する準備ができます。 詳しくは、[「Microsoft 365 のネイティブ モードで Yammer ネットワークを構成する」](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode) を参照してください。