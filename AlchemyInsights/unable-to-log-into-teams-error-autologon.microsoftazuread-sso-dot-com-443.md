---
title: エラー autologon.microsoftazuread-sso.com:443 のため Teams にログインできない
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9001686"
- "3750"
ms.openlocfilehash: 77049153939989d1c63789adfec0b494d047a6e4
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/24/2020
ms.locfileid: "42935330"
---
# <a name="unable-to-log-into-teams-due-to-error-autologonmicrosoftazuread-sso-dot-com443"></a>エラー autologon.microsoftazuread-sso dot com:443 のため Teams にログインできない

シームレス SSO が O365 認証として有効な場合、URL "autologon.microsoftazuread-sso.com" をイントラネット サイトに追加しなければならないことがあります。  信頼済みサイトに既に追加してあり、シームレス SSO を使用している場合には、信頼済みサイトから削除しなければなりません。

[シームレス SSO トラブルシューティングのチェックリスト](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso#troubleshooting-checklist)をご確認ください。

次の手順を使用して、URL をイントラネット サイトの一覧に追加します。

1. **[スタート]** ボタンをクリックして、Internet Explorer を開きます。 検索ボックスに Internet Explorer と入力し、結果の一覧で **Internet Explorer** をクリックします。
2. **[ツール]**、**[インターネット オプション]** の順にクリックします。
3. **[セキュリティ]** タブをクリックします。
4. **[ローカル イントラネット]**、**[サイト]** ボタン、**[詳細設定]** ボタンの順にクリックします。
5. Web サイト URL を入力して、**[追加]** をクリックします。
6. 完了したら、**[閉じる]** をクリックします。

詳細については、[O365 のシームレス SSO の展開に関する資料](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start) (手順 3 の URL をイントラネット サイトに追加するためのポリシー ベースのプロセスを含め) を参照してください。
