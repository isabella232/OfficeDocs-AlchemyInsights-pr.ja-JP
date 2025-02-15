---
title: 監査ログで IP アドレスとクライアントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 57a1756787f8297a2a1ab3012b95aaa2f33e6045
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313024"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>監査ログで IP アドレスとクライアントを識別する

監査ログには、Microsoft 365 ユーザーまたは管理者によるアクティビティに対応する IP アドレスが表示されます。 クライアント情報も記録されます。 ここでは、そのような情報を識別するための手順をご紹介します。

1. [Microsoft 365 コンプライアンス センター](https://protection.office.com/)にログインします。

2. **[検索]** > **[監査ログの検索]** ページに移動します。

   特定のアクティビティに関心がある場合は、[**アクティビティ**] リストから選択します。 そうでない場合は、選択したユーザーのすべての活動が返されます(既定の設定) 。

   **注意**: 特定のアクティビティは、[**アクティビティ**] のメニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示**] が選択されていれば、これらの監査項目が返されます（デフォルト設定）。

3. [**ユーザー**] フィールド内のユーザー名を指定し、アクティビティの適切な日付の範囲を選択し、[**検索**] をクリックします。

結果では、結果ウィンドウでそのアクティビティの IP アドレスを見ることができます。 [**詳細情報**] ポップアップにある [監査記録] を選択し、 詳細な情報 (たとえば、クライアント、アクションを実行したユーザーなど)を表示します。

詳細については [安全性が脅かされたアカウントへのアクセスに使用されたコンピューターの IP アドレスを見つける](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account)を参照してください。
