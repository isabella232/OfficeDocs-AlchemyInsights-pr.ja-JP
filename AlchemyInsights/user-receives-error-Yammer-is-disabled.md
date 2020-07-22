---
title: ユーザーが受け取ったエラー AADSTS7000112 Yammer が無効になっています
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6010"
- "9003111"
ms.openlocfilehash: c92b09ee9a9ca06f85906e7fce601582a7e83244
ms.sourcegitcommit: c078058ee0b77ee1f1496feb2f3a5773e3e3b30d
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2020
ms.locfileid: "45198654"
---
# <a name="user-receives-error-aadsts7000112-yammer-is-disabled"></a>ユーザーが受け取ったエラー AADSTS7000112 Yammer が無効になっています

エラー「AADSTS7000112: Application '00000005-0000-0ff1-ce00-000000000000'(Yammer) is disabled」を受け取った場合は、Azure AD 内のサービスプリンシパルに問題があります。 管理者がサービスプリンシパルを無効にして、Yammer へのアクセスをブロックしている可能性があります。

サービスプリンシパルを無効にすることはお勧めできません。別の問題が発生する恐れがあります。 Yammer へのユーザーアクセスをブロックするためにサポートされているアプローチの詳細については、「[Microsoft 365ユーザーのYammer アクセスを無効にする](https://docs.microsoft.com/yammer/manage-yammer-users/turn-off-user-access)」を参照してください。  

Azure Portal でこの問題を修正し、Yammer へのユーザーアクセスを復元するには：

1.  Azure Active Directory ページを開き、左側のナビゲーションウィンドウの[**管理**]で[**エンタープライズアプリケーション**]を選択します。
3.  検索ボックスに「** Office 365 Yammer **」と入力し、アプリケーション名を選択して設定を開きます。
4.  左側のナビゲーションウィンドウの[**管理**]で[**プロパティ**]を選択します。
5.  [**ユーザーがログインできるようにしますか?**]の値を[**はい**]に設定して、[**保存**]を選択します。
6.  Yammer に再度サインインします。 クッキーを消去する必要があるかもしれません。

または、PowerShell コマンドを実行して値を設定します。 詳細については、Office 365 で Yammer タイルをクリックする際に発生するエラー[「Sorry, but we're having trouble signing you in」](https://docs.microsoft.com/yammer/troubleshoot-problems/error-when-click-the-yammer-tile-in-office-365)を参照してください。 