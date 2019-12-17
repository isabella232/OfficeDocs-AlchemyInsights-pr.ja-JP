---
title: トラブルシューティングの問題 - ディレクトリにユーザーが見つかりません
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 0f1e427801107109e31486a4d300f53084880caf
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/15/2019
ms.locfileid: "40054815"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>トラブルシューティングの問題 - ディレクトリにユーザーが見つかりません

ディレクトリに "ユーザーが見つかりません" というエラーメッセージが表示されている場合は、問題の種類が、"ディレクトリ内にユーザーが見つかりません" のときにもう一度お試しください。

問題のトラブルシューティングを行うには、次の手順を実行します。

- メール招待状を受諾したアカウントが、後でサインインするために使用しているアカウントと同じであることを確認します。 ユーザーが招待を承諾してサイトにサインインするために同じアカウントを使用していることを確認します。 

詳細については、[「Office 365 ログインを管理するために Microsoft アカウント</a>のエイリアスを管理する方法」](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)を参照してください。 

- ユーザーがエラーを受信している各サイトに移動します。 

サイト URL の末尾に "/_layouts/15/people.aspx/membershipgroupid = 0" (二重引用符内) を追加します。 

例: https://<"contoso">.sharepoint.com/_layouts/15/people.aspx/membershipGroupId=0。

- 一覧からユーザーを選択します。

- [**ユーザー権限の削除**] をクリックします。 
-  ユーザーを追加して、ユーザーに招待状を再送信します。

