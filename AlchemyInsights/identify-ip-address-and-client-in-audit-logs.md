---
title: 監査ログで IP アドレスとクライアントを識別する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d1a0d412fc0c6d79e50b101ca759127522f45dcd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716393"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a>監査ログで IP アドレスとクライアントを識別する

監査ログには、Microsoft 365 ユーザーまたは管理者によるアクティビティに対応する IP アドレスが表示されます。 クライアント情報も記録されます。 ここでは、そのような情報を識別するための手順をご紹介します。

1. [Microsoft 365 セキュリティ/コンプライアンス センター](https://protection.office.com/) にログインします。

2. **[検索]** > **[監査ログの検索]** ページに移動します。

   特定のアクティビティに関心がある場合は、[**アクティビティ**] リストから選択します。 そうでない場合は、選択したユーザーのすべての活動が返されます(既定の設定) 。

   **注意**: 特定のアクティビティは、[**アクティビティ**] のメニューに表示されない場合があります。ただし、[**すべてのアクティビティの結果を表示**] が選択されていれば、これらの監査項目が返されます（デフォルト設定）。

3. [**ユーザー**] フィールド内のユーザー名を指定し、アクティビティの適切な日付の範囲を選択し、[**検索**] をクリックします。

結果では、結果ウィンドウでそのアクティビティの IP アドレスを見ることができます。 [**詳細情報**] ポップアップにある [監査記録] を選択し、 詳細な情報 (たとえば、クライアント、アクションを実行したユーザーなど)を表示します。

詳細については [安全性が脅かされたアカウントへのアクセスに使用されたコンピューターの IP アドレスを見つける](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account)を参照してください。
