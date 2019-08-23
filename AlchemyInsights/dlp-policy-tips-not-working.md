---
title: DLP ポリシーのヒントが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 1619d50b98419f59a1f863983c4ec5bff01679b4
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530316"
---
# <a name="dlp-policy-tip-issues"></a>DLP ポリシーのヒントに関する問題

**DLPポリシー**を使用している場合は、**ポリシーのヒント**を使用してポリシー違反をユーザーに通知できます。 管理者は、DLPポリシーをテストしている間、ポリシーが完全実施モードになっているときいずれの場合でも表示されるポリシーのヒントを設定できます。
  
セキュリティ/コンプライアンス センターの完全実施モードでDLPポリシーに関するポリシーのヒントを構成するには、次の手順を実行します：
  
- DLP ルールでポリシー ヒントを**有効**にします。そのためには、[こちら](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)の手順を実行します。

- **コンテンツが、[こちら](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)の記事に略述されているルールをトリガーする**ために**必要な**点を満たしていることを確認します。

- ポリシー ヒントは OWA と Outlook の両方に表示されますが、**Outlook 2013 以降**を使用する場合、ポリシー ヒントが表示されるのは特定の条件下に限定されます。該当する条件については、次の資料に記されています: [ポリシー ヒントを表示するために Outlook 2013 以降でサポートされている条件](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

DLP ポリシー ヒントについての追加情報については、以下をご覧ください: [DLP ポリシーのポリシー ヒントを表示する](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  