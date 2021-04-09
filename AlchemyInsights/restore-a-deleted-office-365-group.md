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
ms.openlocfilehash: caa2c8987eecb89bac3469bf9471847858cab0ba
ms.sourcegitcommit: ec99a3a2e1e6a13d9a829d65ad1692a607dc3a17
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/06/2021
ms.locfileid: "51597448"
---
# <a name="restore-a-deleted-microsoft-365-group"></a>削除された Microsoft 365 グループを復元する

削除された Microsoft 365 グループまたは Microsoft Teams は、削除から 30 日以内なら復元できます。

1. [Microsoft 365 管理センター](https://aka.ms/RestoreDeletedGroup)にアクセスしてログインし、削除したグループとチームを一覧表示します。

    **注:** テナントの管理者またはグループ管理者の役割に割り当てられているアカウントを使用してログインします。

1. 復元する削除済み Microsoft 365 グループ/Teams を選択し、**[グループの復元]** をクリックします。

    SMTP アドレスが競合するためにグループを復元できない場合は、次のコマンドを使用して競合の原因となっているオブジェクトを探し、SMTP アドレスを削除します。

    `Get-Recipient -Filter "EmailAddresses -eq '<conflictingsmtpaddress>'"`

    **注:** グループとそのすべてのデータが完全に復元されるまで 24 時間ほどかかる場合があります。

    詳細な情報、または PowerShell を使用したグループの復元方法については、「[削除された Microsoft 365 グループを復元する](https://go.microsoft.com/fwlink/?linkid=867802)」を参照してください。