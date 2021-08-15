---
title: ClientAccessServerEnabled を True に設定する
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: b134c952e3cc5305d8f3e6f44031e7f33d7938b67ff122c46cb74bbd33cbf59e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994870"
---
# <a name="set-clientaccessserverenabled-to-true"></a>ClientAccessServerEnabled を True に設定する

暗号化されたメール メッセージを開くことができず、代わりに **rpmsg** の添付ファイルが表示される場合は、次の手順を実行します。

1. Exchange Online PowerShell に接続します。

> [!NOTE]
> Exchange Online PowerShell に接続するには、グローバル管理者または Exchange 管理者アカウントを使用してサインインする必要があります。

   a. Windows PowerShell を開き、次のコマンドを実行します: `$UserCredential = Get-Credential`
b. **[Windows PowerShell 資格情報の要求]** ダイアログ ボックスで、職場または学校のアカウントとパスワードを入力します。 **[OK]** をクリックします。 

2. 次のコマンドを実行して、新しいセッションを作成します。

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    a. 次のコマンドを実行します。
    
    `Import-PSSession $Session -DisableNameChecking`

3. `Get-IRMConfiguration` コマンドを実行します。

4. **ClientAccessServerEnabled** 設定を確認します。 

    a. **ClientAccessServerEnabled** 設定が **False** に設定されている場合は、次のコマンドレットを実行します: `Set-IRMConfiguration -ClientAccessServerEnabled $True`

> [!TIP]
> 次のコマンドを使用して、PowerShell セッションを常に閉じます: `Remove-PSSession $Session`

詳細については、「[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)」をご覧ください。

