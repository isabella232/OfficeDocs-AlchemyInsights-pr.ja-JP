---
title: DLP ポリシーのヒントが機能しない
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 9369878b62a5abe79bd215487bea6cabb0e80f06
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507447"
---
# <a name="dlp-policy-tip-issues"></a>DLP ポリシーのヒントに関する問題

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**DLP ポリシーのヒント**

**DLPポリシー**を使用している場合は、**ポリシーのヒント**を使用してポリシー違反をユーザーに通知できます。 管理者は、DLPポリシーをテストしている間、ポリシーが完全実施モードになっているときいずれの場合でも表示されるポリシーのヒントを設定できます。
  
セキュリティ/コンプライアンス センターの完全実施モードでDLPポリシーに関するポリシーのヒントを構成するには、次の手順を実行します：
  
- DLP ルールでポリシー ヒントを**有効**にします。そのためには、[こちら](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)の手順を実行します。

- **コンテンツが、[こちら](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)の記事に略述されているルールをトリガーする**ために**必要な**点を満たしていることを確認します。

- Policy tips display in both OWA and Outlook. However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions. These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)

DLP ポリシー ヒントについての追加情報については、以下をご覧ください: [DLP ポリシーのポリシー ヒントを表示する](https://docs.microsoft.com/microsoft-365/compliance/use-notifications-and-policy-tips)
  