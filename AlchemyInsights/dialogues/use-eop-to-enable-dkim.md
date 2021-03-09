---
title: Exchange Online PowerShell を使用して特定のドメインに対して DKIM を有効にする
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/23/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: 2f2b60a63b512bde794ba588852db11423e766f3
ms.sourcegitcommit: 78fe9f33438cb0c19f0dab31253b5853b73f4f47
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527790"
---
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a>Exchange Online PowerShell を使用して特定のドメインに対して DKIM を有効にする

管理センターで DKIM DNS レコードを作成できない場合は、Exchange Online PowerShell を使用してみてください。 

Exchange Online PowerShell を使用して DKIM DNS レコードを作成するには、次の手順を実行します。

1. 管理者として Windows PowerShell を開き、以下のコマンドを説明順に実行します。

    a.  `$UserCredential = Get-Credential`

    b.  `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    c. `Import-PSSession $Session -DisableNameChecking`
    
Exchange Online PowerShell に接続できない場合は、「[Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)」を参照してください。

2. Exchange Online PowerShell に接続したら、次のコマンドを実行します。

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. 上記のコマンドが正常に実行されたら、次のコマンドを実行して Exchange Online PowerShell のセッションを終了します。

    `Remove-PSSession $Session` 



