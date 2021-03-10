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
ms.openlocfilehash: 2adf35662797e9e9e354ddd0c513f5ce2463d07c
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/05/2021
ms.locfileid: "50527855"
---
# <a name="set-clientaccessserverenabled-to-true"></a><span data-ttu-id="c5957-102">ClientAccessServerEnabled を True に設定する</span><span class="sxs-lookup"><span data-stu-id="c5957-102">Set ClientAccessServerEnabled to True</span></span>

<span data-ttu-id="c5957-103">暗号化されたメール メッセージを開くことができず、代わりに **rpmsg** の添付ファイルが表示される場合は、次の手順を実行します。</span><span class="sxs-lookup"><span data-stu-id="c5957-103">If you can't open an encrypted email message and instead see an **rpmsg** attachment, perform the following steps:</span></span>

1. <span data-ttu-id="c5957-104">Exchange Online PowerShell に接続します。</span><span class="sxs-lookup"><span data-stu-id="c5957-104">Connect to Exchange Online PowerShell.</span></span>

> [!NOTE]
> <span data-ttu-id="c5957-105">Exchange Online PowerShell に接続するには、グローバル管理者または Exchange 管理者アカウントを使用してサインインする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c5957-105">To connect to Exchange Online PowerShell, you must sign in using a global admin or Exchange admin account.</span></span>

   <span data-ttu-id="c5957-106">a.</span><span class="sxs-lookup"><span data-stu-id="c5957-106">a.</span></span> <span data-ttu-id="c5957-107">Windows PowerShell を開き、次のコマンドを実行します: `$UserCredential = Get-Credential`</span><span class="sxs-lookup"><span data-stu-id="c5957-107">Open Windows PowerShell, and then run the following command: `$UserCredential = Get-Credential`</span></span>
<span data-ttu-id="c5957-108">b.</span><span class="sxs-lookup"><span data-stu-id="c5957-108">b.</span></span> <span data-ttu-id="c5957-109">**[Windows PowerShell 資格情報の要求]** ダイアログ ボックスで、職場または学校のアカウントとパスワードを入力します。</span><span class="sxs-lookup"><span data-stu-id="c5957-109">In the **Windows PowerShell Credential Request** dialog box, enter your work or school account and password, c.</span></span> <span data-ttu-id="c5957-110">**[OK]** をクリックします。</span><span class="sxs-lookup"><span data-stu-id="c5957-110">Click **OK**.</span></span> 

2. <span data-ttu-id="c5957-111">次のコマンドを実行して、新しいセッションを作成します。</span><span class="sxs-lookup"><span data-stu-id="c5957-111">Run the following command to create a new session:</span></span>

    `$Session = New-PSSession -ConfigurationName Microsoft.Exchange -ConnectionUri https://outlook.office365.com/powershell-liveid/ -Credential $UserCredential -Authentication Basic -AllowRedirection`

    <span data-ttu-id="c5957-112">a.</span><span class="sxs-lookup"><span data-stu-id="c5957-112">a.</span></span> <span data-ttu-id="c5957-113">次のコマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="c5957-113">Run the following command:</span></span>
    
    `Import-PSSession $Session -DisableNameChecking`

3. <span data-ttu-id="c5957-114">`Get-IRMConfiguration` コマンドを実行します。</span><span class="sxs-lookup"><span data-stu-id="c5957-114">Run `Get-IRMConfiguration` command.</span></span>

4. <span data-ttu-id="c5957-115">**ClientAccessServerEnabled** 設定を確認します。</span><span class="sxs-lookup"><span data-stu-id="c5957-115">Check the **ClientAccessServerEnabled** setting.</span></span> 

    <span data-ttu-id="c5957-116">a.</span><span class="sxs-lookup"><span data-stu-id="c5957-116">a.</span></span> <span data-ttu-id="c5957-117">**ClientAccessServerEnabled** 設定が **False** に設定されている場合は、次のコマンドレットを実行します: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span><span class="sxs-lookup"><span data-stu-id="c5957-117">If **ClientAccessServerEnabled** setting is set to **False**, run the following cmdlet: `Set-IRMConfiguration -ClientAccessServerEnabled $True`</span></span>

> [!TIP]
> <span data-ttu-id="c5957-118">次のコマンドを使用して、PowerShell セッションを常に閉じます: `Remove-PSSession $Session`</span><span class="sxs-lookup"><span data-stu-id="c5957-118">Always close your powershell session with the following command: `Remove-PSSession $Session`</span></span>

<span data-ttu-id="c5957-119">詳細については、「[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="c5957-119">For more information, see [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell).</span></span>

