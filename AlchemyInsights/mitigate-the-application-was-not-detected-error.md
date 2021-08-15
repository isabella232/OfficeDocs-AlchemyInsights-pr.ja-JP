---
title: アプリケーションが検出されなかったエラーを軽減する
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026119"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>"アプリケーションが見つかりませんでした" というエラーを軽減する

Intune によって報告されたアプリ インストール エラー、 "インストールが正常に完了した後、アプリが検出されませんでした”は、すべての主要な OS プラットフォーム (Windows、iOS、Android) で発生する可能性があります。

このエラーが発生する最も一般的なシナリオは次のとおりです。

- 初期展開後、アプリは Intune の外部(サードパーティのアプリストア)で更新されている場合。 たとえば、Google Chrome などの一部のアプリケーションは、自動更新が実行される場合があります。
- ユーザーが、最初にインストールした後にアプリをアンインストールした場合。

この問題を軽減するには、まず、影響を受けるデバイスを確認して、エラーが発生するシナリオを特定します。

- アプリが Intune 以外で更新されている場合は、アプリケーションのバージョンを無視するようにアプリの展開の設定ができます。 この設定を行うには、**[アプリ構成] > [アプリの情報]** で、**[アプリのバージョンを無視]** を [**はい**] に設定します。
- クライアントを対象としている場合は、"必須" としてアプリケーションを展開して、最新バージョンが展開されていることを確認します。
- または、iOS プラットフォームでは、Apple Volume Purchase Program に関連付けられている **autoupdate** 機能を使用できます。これは、新しいアプリケーション バージョンが利用可能になったときに自動的に更新されるように構成できます。

アプリのインストールに関する問題のトラブルシューティングの詳細については、「[アプリのインストールの問題のトラブルシューティング](https://docs.microsoft.com/intune/troubleshoot-app-install)」を参照してください。
