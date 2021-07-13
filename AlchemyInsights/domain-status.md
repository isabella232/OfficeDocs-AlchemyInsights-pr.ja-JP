---
title: ドメイン ステータス - サービスが選択されていません
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11094"
- "9006491"
ms.openlocfilehash: 66fae5b5602dd67954ac9208b26bc2005adda0e3
ms.sourcegitcommit: 56650eb9af437ff97e4f4d9ca5a2f53ad5bb990e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/12/2021
ms.locfileid: "53389186"
---
# <a name="domain-status---no-services-selected"></a>ドメイン ステータス - サービスが選択されていません

**サービスが選択** されていないことは、Exchange Online、Skype for Business、Intune などの Microsoft 365 サービス、Microsoft 365 がカスタム ドメインで使用するモバイル デバイス管理を選択していないという意味です。 Exchange ハイブリッド (Exchange オンプレミス Exchange Online) または Exchange と他の Microsoft サービス を使用した外部スパム フィルターを使用している場合は、このメッセージを無視できます。 ドメインの正常性状態は、サービスに直接接続されているドメインでのみ使用できます。

ドメインのサービスを選択するには、次の方法を実行します。

1. **[設定** ドメイン] で、状態メッセージ [サービスなし] が選択されているドメインの横  >  [](https://admin.microsoft.com/Adminportal/Home)にあるボックス **をオンにします**。
1. [DNS **の管理] を** 選択して、ドメイン セットアップ ウィザードを開始します。
    - [独自の **DNS レコードを追加する] を選択した** 場合は、メッセージが表示されたら必ずサービスを選択してください。 その他のサービスは、[高度なオプション] **で利用できます**。
    - [Microsoft に **DNS レコード** を追加する] または [その他のオプションを設定する] を選択すると、利用可能なすべてのサービスが自動的に  >  提案され、選択されます。
1. ウィザードに進み、DNS セットアップとサービスの選択肢を完了します。
 
ドメインの設定に関するその他のヘルプについては、「 [ドメインに接続するための DNS レコードの追加」を参照してください](/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)。

