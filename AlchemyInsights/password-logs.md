---
title: パスワード ログ
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ab2899cc96fb76705665eff4a535de5ada5bc4dd733723349a6fb649adfb034b
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53960948"
---
# <a name="password-logs"></a>パスワード ログ

**パスワード リセットの監査ログへのアクセスに問題が発生しています**。

パスワード リセット監査ログへのアクセスに関する問題を解決するには、次の手順を実行します。

監査ログを表示する権限があることを確認します。 

次のロールのみ認証されています。
 - グローバル管理者
 - セキュリティ管理者
 - セキュリティ閲覧者

**最初に展開したときからのすべてのパスワード リセット監査イベントを確認したい**

過去 30 日間のレポートには、最大 12 万件のパスワード リセット/登録イベントが保存されています。 この上限は CSV をダウンロードする場合の UI に適用されます。 100 万件のイベントが PowerShell から利用可能です。
詳細については、以下のリンクを参照してください。

- [Azure AD Reports and Events API でのセルフサービスのパスワード リセット イベント](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [PowerShell を使用してパスワード リセット登録イベントを素早くダウンロードする方法](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

**パスワード リセットのレポート機能について詳しく知りたい**

Azure ポータルの **[ユーザーとグループ]** の Azure AD パスワード リセット監査ログで、登録しているユーザーやパスワードをリセットしているユーザーを確認します。
詳細については、以下のリンクを参照してください。

- [パスワード リセット レポートの概要](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Azure ポータルでパスワード リセット レポートを表示する方法](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [Azure AD Reports and Events API でのセルフサービスのパスワード リセット イベント](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [PowerShell を使用してパスワード リセット登録イベントを素早くダウンロードする方法](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


