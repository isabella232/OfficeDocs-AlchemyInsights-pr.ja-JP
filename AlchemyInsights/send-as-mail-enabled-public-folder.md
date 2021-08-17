---
title: EXO でメールが有効なパブリック フォルダーとして送信する
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: 22aa3e8f46c2ff4f62cb520b9498041dffb9d3a3eb607d788cc97b10bf32dbb5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "54052571"
---
# <a name="sendas-mail-enabled-public-folder"></a>メールが有効なパブリック フォルダーとして送信する

次の例では、メールが有効なパブリック フォルダー NewPF1 の "差出人を指定して送信する" アクセス許可をユーザー Jason に割り当てています。

Add-RecipientPermission -Identity "NewPF1" -Trustee "Jason" -AccessRights "SendAs"

詳細な構文やパラメーターの情報については、「[メールが有効なパブリック フォルダーに "差出人を指定して送信する" または "代理人として送信する" アクセス許可を割り当てる](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs)」を参照してください。

