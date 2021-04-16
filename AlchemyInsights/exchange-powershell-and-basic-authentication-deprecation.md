---
title: Exchange PowerShell と基本認証の廃止
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500011"
- "4577"
ms.openlocfilehash: 01938a59b53ccf8b7867ed9c256e141205d31dff
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813477"
---
# <a name="exchange-powershell-and-basic-authentication-deprecation"></a><span data-ttu-id="91962-102">Exchange PowerShell と基本認証の廃止</span><span class="sxs-lookup"><span data-stu-id="91962-102">Exchange PowerShell and basic authentication deprecation</span></span>

<span data-ttu-id="91962-103">基本認証を使用せずに Exchange Online PowerShell に接続する方法についての最新情報は、[こちらを参照してください](https://aka.ms/exops-docs)。</span><span class="sxs-lookup"><span data-stu-id="91962-103">For the latest information about how to connect to Exchange Online PowerShell without the use of Basic Authentication, [please go here](https://aka.ms/exops-docs).</span></span> <span data-ttu-id="91962-104">PowerShell V2 モジュールは基本認証を使用しません。</span><span class="sxs-lookup"><span data-stu-id="91962-104">The PowerShell V2 module does not use basic authentication.</span></span>

<span data-ttu-id="91962-105">クライアント コンピューターで基本認証を有効にする必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="91962-105">Please note that Basic Authentication still needs to be enabled on your client machine.</span></span>
<span data-ttu-id="91962-106">新しい PowerShell V2 モジュールは、先進認証を使用して、すべての REST ベースの V2 コマンドレットを有効にするための接続を確立します。</span><span class="sxs-lookup"><span data-stu-id="91962-106">The new PowerShell V2 module uses Modern Auth to establish connection for enabling all of REST-based V2 Cmdlets.</span></span> <span data-ttu-id="91962-107">V2 コマンドレットに加えて、リモート PowerShell セッションを確立する必要がある古いリモート PowerShell (RPS) コマンドレットにアクセスすることもできます。</span><span class="sxs-lookup"><span data-stu-id="91962-107">In addition to V2 cmdlets, it also allows you to access older Remote PowerShell (RPS) Cmdlets which requires a Remote PowerShell session to be established.</span></span> <span data-ttu-id="91962-108">Windows コンピューターで RPS セッションを確立するには、モジュールが先進認証メカニズムを使用してサービスを認証する場合でも、クライアント コンピューターで WinRM 基本認証を有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="91962-108">Establishing an RPS session on Windows machine requires WinRM BasicAuth to be enabled on the client machine even though the module uses Modern Auth mechanism to authenticate to the service.</span></span> <span data-ttu-id="91962-109">WinRM 基本認証パイプラインは、先進認証トークンの転送に使用されます。</span><span class="sxs-lookup"><span data-stu-id="91962-109">The WinRM Basic Auth pipeline is used for transporting Modern Auth tokens.</span></span> <span data-ttu-id="91962-110">クライアント コンピューターで WinRM 基本認証が無効になっている場合、新しい V2 コマンドレットは引き続き機能します (ただし、古い RPS コマンドレットは機能しません)。</span><span class="sxs-lookup"><span data-stu-id="91962-110">If WinRM Basic Auth is disabled on the client machine, the new V2 cmdlets will continue to work (but the older RPS cmdlets will not).</span></span>
