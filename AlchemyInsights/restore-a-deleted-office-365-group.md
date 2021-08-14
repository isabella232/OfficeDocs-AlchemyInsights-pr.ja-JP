---
title: 削除された Microsoft 365 グループを復元する
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "98"
- "1200024"
ms.assetid: bc0396ea-c426-4d1d-bb89-ced602d06fb6
ms.openlocfilehash: 6262ca04335c355fb4de41a9e1d854b666f47e10321a843717d6eb951c46cafd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53959031"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>削除された Microsoft 365 グループを復元する

削除された Microsoft 365 グループまたは Microsoft Teams は、削除から 30 日以内なら復元できます。

1. [Microsoft 365 管理センター](https://aka.ms/RestoreDeletedGroup)にアクセスして、削除されたグループとチームのリストにログインします。

    **注:** テナントの管理者またはグループ管理者の役割に割り当てられているアカウントを使用してログインします。

1. 復元する削除済み Microsoft 365 グループ/Teams を選択し、**[グループの復元]** をクリックします。

    SMTP アドレスが競合するためにグループを復元できない場合は、次のコマンドを使用して競合の原因となっているオブジェクトを探し、SMTP アドレスを削除します。

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **注:** グループとそのすべてのデータが完全に復元されるまで 24 時間ほどかかる場合があります。

    詳細な情報、または PowerShell を使用したグループの復元方法については、「[削除された Microsoft 365 グループを復元する](https://go.microsoft.com/fwlink/?linkid=867802)」を参照してください。