---
title: OneDrive for Business Web OneDrive を Delve にリダイレクトする
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922992"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>[OneDrive] をクリックした後、Delve にリダイレクトされる

詳細については、「[トラブルシューティング ガイド](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)」を参照してください。

この問題を解決するには、管理者は、ユーザーに [個人用サイト] サイトを作成する権限を付与する必要があります。 これは、OneDrive for Business ページが個人用サイトに作成されているためです。

この権限を付与するには、次の手順を実行します。

1. SharePoint 管理センターで、[**ユーザー プロファイル**] をクリックします。

2. [**ひと**] セクションで、 [**ユーザー権限の管理**] をクリックします。

3. [個人用サイト] サイトを作成する権限を必要とするユーザーを追加します。 既定では、この設定は [**外部ユーザー以外のすべてのユーザー**] に設定されます。

4. ユーザー、複数のユーザー、またはグループを追加したら、追加したユーザー、複数のユーザー、またはグループが選択されていることを確認して、[**アクセス許可**] セクションまでスクロールして、[**個人用サイトの作成 (個人用ストレージ、ニュースフィード、およびフォローしたコンテンツ)**] の隣のチェック ボックスを選択します。

5. [**OK**] をクリックし、ユーザーに OneDrive ページに移動してサイトを作成してもらいます。
