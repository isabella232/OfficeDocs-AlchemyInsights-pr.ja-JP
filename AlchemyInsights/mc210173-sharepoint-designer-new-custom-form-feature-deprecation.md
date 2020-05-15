---
title: MC210173 - SharePoint Designer の新しいユーザー設定フォーム機能の廃止
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 185e8fc94345b240667490b1ffc63af8459d8daf
ms.sourcegitcommit: a9e6b2fcce8bd12fd079ed967f426b67d5c6d239
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/28/2020
ms.locfileid: "43935032"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - SharePoint Designer の新しいユーザー設定フォーム機能の廃止

Sharepoint Online 内で[ユーザー設定 フォームを作成する](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2)に対して、SharePoint Designer の機能に影響する問題が特定されました。 慎重に調査したところ、この問題の修正はありませんが、2020 年 4 月 25 日 土曜日 午前 3 時 UTC 現在をもって、ユーザー設定のフォームの作成機能を無効を選択することをお勧めします。 この変更は、以前に作成したフォームや、SharePoint Online デザイナーのその他の既存の機能を編集するのに影響はありません。

この変更を行うと、新しいフォームを作成するときに、"サーバーに変更を保存できませんでした" というエラーが表示されることがあります。

ユーザー設定のフォームを作成するのに以前 SharePoint Designer を活用していたユーザーは、代わりにこの目的のために[PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form)を使用できます。

PowerApps は、SharePoint Online の最新の機能を操作しているユーザーが、ブラウザー ウィンドウから SharePoint リストおよびドキュメント ライブラリのユーザー設定フォームを作成および編集できる、簡単で強力なツールです。 PowerApps では、従来のコーディング知識や、InfoPath など任意の追加のアプリのダウンロードは必要ありません。

**注**SharePoint Online の従来のユーザーは、PowerApps にアクセスして使用するために、最新のエクスペリエンスに一時的に切り替える必要があります。ただし、PowerApps で作成されるすべてのユーザー設定フォームには、SharePoint Online のクラシック エクスペリエンス ユーザーがアクセスできます。
