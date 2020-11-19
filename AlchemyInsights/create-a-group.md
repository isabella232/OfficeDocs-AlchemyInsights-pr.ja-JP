---
title: グループを作成する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/17/2020
ms.locfileid: "49089267"
---
# <a name="create-a-group"></a>グループを作成する

このトピックでは、グループの作成について説明します。

**グループを作成する権限**

新しいグループを作成する権限があることを確認します。 グローバル管理者は、Azure ポータルまたはアクセス パネルでグループの作成を無効にできます。 新しいグループを作成したり、適切な権限を付与したりするには、管理者が必要になる場合があります。

**グループ作成の権限の管理**

1. グローバル管理者は、**[すべてのグループ]** >  **[全般 (設定)]** で「ユーザーは Azure ポータルでセキュリティ グループを作成できます」または「ユーザーは Azure ポータルで Office 365 グループを作成できます」オプションを選択することにより、グループ作成のアクセス許可 (セキュリティ上の理由)、Azure ポータル、またはアクセスパネルで作成された Office 365 グループを管理できます。
2. Azure Active Directory P1 Premium ライセンスをお持ちの場合は、グループの作成を制限してユーザーのグループを選択することもできます。

**新しい Office 365 グループメンバーのウェルカム通知を無効にする**

Office 365 グループに追加されたユーザーに送信されるウェルカム通知を無効にするには、Powershell で **UnifiedGroupWelcomeMessageEnabled** を False に設定します。 この設定については、[こちら](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)をご覧ください。

