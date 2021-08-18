---
title: Teams の連絡先の同期
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
- "9004610"
- "11540"
ms.openlocfilehash: efc1f29c6e2f76d763f2f8102db7e9f6afb1f1be
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58327338"
---
# <a name="teams-contacts-sync"></a>Teams の連絡先の同期

Teams では、組織の Active Directory の連絡先、およびユーザーの Outlook の既定のフォルダーに追加された連絡先を使用します。 連絡先が Microsoft Teams に表示されない場合は、次のことを試してください。

**注:** 1 つ以上の連絡先の情報が最近更新された場合、連絡先が同期されるまでに最大 48 時間かかる場合があります。

1. Teams からログアウトして再起動します。 連絡先が表示されるかどうかを確認します。
1. Teams のキャッシュをクリアします。
    1. **%appdata%\Microsoft\Teams** に移動します。
    1. フォルダーの内容を削除します。
    1. コンピューターを再起動し、Teams を起動します。
1. 連絡先が Outlook にある場合は、必ず連絡先リストに追加してください。 Outlook で、アドレス バーから **[ファイル]** を選択し、**[連絡先に追加]** を選択します。
1. ユーザーの Exchange メールボックスが (オンプレミスではなく) オンラインでホストされていることを確認してください。 詳細については、「[Exchange と Microsoft Teams の連携](https://docs.microsoft.com/microsoftteams/exchange-teams-interact)」を参照してください。
1. 連絡先の電話番号が連絡先情報に追加されていることを確認します。
1. [検索] バーで連絡先のメールを検索します。 連絡先リストへの同期を取得できる連絡先。
