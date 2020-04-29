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
ms.openlocfilehash: 7d31f6bcbd464b7428092b6fd6ff9f9582db2a8b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704382"
---
# <a name="dlp-policy-tip-issues"></a>DLP ポリシーのヒントに関する問題

**重要**: これらの前例のない時期にも、SharePoint Online および OneDrive サービスの可用性を維持するための措置を講じています。詳細については、「[SharePoint Online の一時的な機能調整](https://aka.ms/ODSPAdjustments)」を参照してください。

**DLP ポリシーのヒント**

**DLPポリシー**を使用している場合は、**ポリシーのヒント**を使用してポリシー違反をユーザーに通知できます。 管理者は、DLPポリシーをテストしている間、ポリシーが完全実施モードになっているときいずれの場合でも表示されるポリシーのヒントを設定できます。
  
セキュリティ/コンプライアンス センターの完全実施モードでDLPポリシーに関するポリシーのヒントを構成するには、次の手順を実行します：
  
- DLP ルールでポリシー ヒントを**有効**にします。そのためには、[こちら](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)の手順を実行します。

- **コンテンツが、[こちら](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)の記事に略述されているルールをトリガーする**ために**必要な**点を満たしていることを確認します。

- ポリシー ヒントは OWA と Outlook の両方に表示されますが、**Outlook 2013 以降**を使用する場合、ポリシー ヒントが表示されるのは特定の条件下に限定されます。該当する条件については、次の資料に記されています: [ポリシー ヒントを表示するために Outlook 2013 以降でサポートされている条件](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

DLP ポリシー ヒントについての追加情報については、以下をご覧ください: [DLP ポリシーのポリシー ヒントを表示する](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  