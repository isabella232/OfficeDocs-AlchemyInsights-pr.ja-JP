---
title: Exchange PowerShell と基本認証の廃止
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 24d59860732b42e8d62da8c1a8c37f2018a0d126
ms.sourcegitcommit: a98b25fa3cac9ebba983f4932881d774880aca93
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2020
ms.locfileid: "44015694"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="d5b5d-102">Exchange PowerShell と基本認証の廃止</span><span class="sxs-lookup"><span data-stu-id="d5b5d-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="d5b5d-103">基本認証を使用せずに Exchange Online PowerShell に接続する方法についての最新情報は、[こちらを参照してください](https://aka.ms/psbasicauth)。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/psbasicauth).</span></span>

<span data-ttu-id="d5b5d-104">クライアント コンピューターで基本認証を有効にする必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-104">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="d5b5d-105">新しい PowerShell V2 モジュールは、先進認証を使用して、すべての REST ベースの V2 コマンドレットを有効にするための接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-105">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="d5b5d-106">V2 コマンドレットに加えて、リモート PowerShell セッションを確立する必要がある古いリモート PowerShell (RPS) コマンドレットにアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-106">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="d5b5d-107">Windows コンピューターで RPS セッションを確立するには、モジュールが先進認証メカニズムを使用してサービスを認証する場合でも、クライアント コンピューターで WinRM 基本認証を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-107">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="d5b5d-108">WinRM 基本認証パイプラインは、先進認証トークンの転送に使用されます。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-108">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="d5b5d-109">クライアント コンピューターで WinRM 基本認証が無効になっている場合、新しい V2 コマンドレットは引き続き機能します (ただし、古い RPS コマンドレットは機能しません)。</span><span class="sxs-lookup"><span data-stu-id="d5b5d-109">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
