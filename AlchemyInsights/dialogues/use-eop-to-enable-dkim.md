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
# <a name="use-exchange-online-powershell-to-enable-dkim-for-a-specific-domain"></a><span data-ttu-id="85180-102">Exchange Online PowerShell を使用して特定のドメインに対して DKIM を有効にする</span><span class="sxs-lookup"><span data-stu-id="85180-102">Use Exchange Online PowerShell to enable DKIM for a specific domain</span></span>

<span data-ttu-id="85180-103">管理センターで DKIM DNS レコードを作成できない場合は、Exchange Online PowerShell を使用してみてください。</span><span class="sxs-lookup"><span data-stu-id="85180-103">If you can't create the DKIM DNS records in the admin center, try using Exchange Online PowerShell.</span></span> 

<span data-ttu-id="85180-104">Exchange Online PowerShell を使用して DKIM DNS レコードを作成するには、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="85180-104">To create a DKIM DNS record using Exchange Online PowerShell, perform the following steps:</span></span>

1. <span data-ttu-id="85180-105">管理者として Windows PowerShell を開き、以下のコマンドを説明順に実行します。</span><span class="sxs-lookup"><span data-stu-id="85180-105">Open Windows PowerShell as an administrator and run the following commands in the described sequence:</span></span>

    <span data-ttu-id="85180-106">a. </span><span class="sxs-lookup"><span data-stu-id="85180-106">a.</span></span> `$UserCredential = Get-Credential`

    <span data-ttu-id="85180-107">b. </span><span class="sxs-lookup"><span data-stu-id="85180-107">b.</span></span> `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="85180-108">c.</span><span class="sxs-lookup"><span data-stu-id="85180-108">c.</span></span> `Import-PSSession $Session -DisableNameChecking`
    
<span data-ttu-id="85180-109">Exchange Online PowerShell に接続できない場合は、「[Exchange Online PowerShell に接続する](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="85180-109">If you have trouble connecting to Exchange Online PowerShell, see [Connect to Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="85180-110">Exchange Online PowerShell に接続したら、次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="85180-110">Once you're connected to Exchange Online PowerShell, run the following command:</span></span>

    `New-DkimSigningConfig -DomainName < CustomDomain > -Enabled $true`

3. <span data-ttu-id="85180-111">上記のコマンドが正常に実行されたら、次のコマンドを実行して Exchange Online PowerShell のセッションを終了します。</span><span class="sxs-lookup"><span data-stu-id="85180-111">Once the above command has been successfully executed, run the following command to terminate the Exchange Online PowerShell session:</span></span>

    `Remove-PSSession $Session` 



