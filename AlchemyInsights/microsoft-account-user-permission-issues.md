---
title: 共有メールボックスを作成および使用する
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.openlocfilehash: 81bf8082198de1c44037291f23c434d06a77f02a
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/07/2019
ms.locfileid: "35174511"
---
# <a name="troubleshoot-issue---user-not-found-in-directory"></a>問題のトラブルシューティング-ディレクトリにユーザーがありません

ユーザーがディレクトリに "ユーザーが見つかりません" というエラーメッセージが表示される場合。 問題の種類がディレクトリ内にない場合は、もう一度やり直してください。

問題のトラブルシューティングを行うには、次の手順を実行します。

- 電子メール招待状を受諾したアカウントが、後でサインインするために使用されているのと同じアカウントであることを確認します。 ユーザーが同じアカウントを使用して、招待状を承諾してサイトにサインインしていることを確認します。 

詳細については、「 [office 365 ログインを管理する</a>ために Microsoft アカウントのエイリアスを管理する方法](https://support.microsoft.com/help/12407/microsoft-account-how-to-manage-aliases)」を参照してください。 

- ユーザーがエラーを受信している各サイトを参照します。 

サイト URL の末尾に "/_layouts/15/people.aspx/membershipgroupid = 0" (二重引用符内) を追加します。 

例: https://< "contoso" >

- リストからユーザーを選択します。

- リボンから [**ユーザー権限の削除**] をクリックします。 
-  ユーザーを再度追加して、招待状を再送信します。

