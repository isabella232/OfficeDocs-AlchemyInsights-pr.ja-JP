---
title: TeamViewer を使用して Intune デバイスをリモート管理する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2020
ms.locfileid: "46556220"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>TeamViewer を使用して Intune デバイスをリモート管理する

Intune で管理されているデバイスは、[TeamViewer](https://www.teamviewer.com/) を使用してリモート管理できます。

TeamViewer を使用して Intune を管理するには、次の手順を実行します。 

まず、TeamViewer から資格情報を取得して、Intune で TeamViewer Connector をセットアップします。 これにより、管理者は、[デバイス] の TeamViewer Connector UI で資格情報を入力できるようになります。これは、Intune と TeamViewer サービスのリンクを確立するための 1 回限りの操作です。

**パート 1: リモート デバイスとのセッションを開始する**

1. [**すべてのデバイス**] で、リモート セッションを開始するデバイスを選択します。
2. [**その他**] で、[**新しいリモート アシスタンス セッション**] を選択します。
3. [**はい**] を選択して、リモート セッションを開始することを確認します。
    "新しいリモート セッションの開始" 要求が TeamViewer サービスによって確認されると、デバイスの [概要] (または [必須項目]) ウィンドウの詳細覧に [**リモート アシスタンスを開始**] というオプションが表示されます。 [**さらに表示**] を選択してウィンドウを展開し、[リモート アシスタンス] の状態を表示します。
4. [**リモート セッションの開始**] を選択して管理者側でセッションを開始します。
5. TeamViewer バイナリ (Windows) をダウンロードすることを選択し、[**実行**] を選択します。<br/>
    **注** TeamViewer Web サイトに開かれるいずれの Web ブラウザーのページも無視します。

6. TeamViewer アプリがデバイスに変更を加えることに関する要求に同意します (Windows のみ)。
7. TeamViewer アプリが起動し、リモート デバイスへの接続を認証するためのセッション コードが提供されます。

**パート 2: リモート セッションの対象デバイスでの操作**

1. Intune の企業ポータルを開きます。
2. "Your IT administrator is requesting control of this device for a remote assistance session (IT 管理者がリモート アシスタンス セッションのためにこのデバイスの制御を要求しています)" という通知フラグを見つけ、この通知を選択します。
3. TeamViewer アプリケーションをダウンロードすることを選択するか、App Store から TeamViewer アプリをダウンロードすることに同意し、[**実行**] を選択します。
    **注** TeamViewer Web サイトに開かれるいずれの Web ブラウザーのページも無視します。

4. TeamViewer アプリがデバイスに変更を加えることに関する要求に同意します (Windows のみ)。
5. TeamViewer アプリが起動し、リモート デバイスへの接続を認証するためのセッション コードが提供されます。
6. ポップアップ ウィンドウが表示され、セッションの開始を許可するかどうかの確認が求められます。

**注**: TeamViewer サービスによって生成されるセッション コードは、1 回限り使用できます。 接続が切れた場合は、次の操作を実行します。

1. リモート デバイスおよび管理ワークステーション上で、TeamViewer アプリのインスタンスを閉じます。
2. リモート デバイスで企業ポータルを閉じます。
3. 管理ポータルから [新しいリモート アシスタンス セッション] を開始します。
4. リモート デバイスで企業ポータルをもう一度開き、新しい通知を受け取ります。
5. 先ほどと同様、リモート デバイスと管理ワークステーションの両方で、TeamViewer アプリを開きます。