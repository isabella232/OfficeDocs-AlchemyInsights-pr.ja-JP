---
title: パスワード同期のトラブルシューティング
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387882"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="eac89-102">パスワード同期のトラブルシューティング</span><span class="sxs-lookup"><span data-stu-id="eac89-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="eac89-103">パスワードの同期の問題をトラブルシューティングするには、この AAD Connect のトラブルシューティングタスクを使用して、パスワードが同期されない理由を特定します。</span><span class="sxs-lookup"><span data-stu-id="eac89-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="eac89-104">開始するには、[直接同期を管理](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement)に移動します。</span><span class="sxs-lookup"><span data-stu-id="eac89-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="eac89-105">Azure AD Connect サーバーで新しい Windows PowerShell セッションを開いて、[**管理者として実行**] オプションを選択します。</span><span class="sxs-lookup"><span data-stu-id="eac89-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="eac89-106">Set-ExecutionPolicy RemoteSigned または Set-ExecutionPolicy Unrestricted を実行します。</span><span class="sxs-lookup"><span data-stu-id="eac89-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="eac89-107">Azure AD Connect ウィザードを開始します。</span><span class="sxs-lookup"><span data-stu-id="eac89-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="eac89-108">追加のタスクページ ＞ **トラブルシューティング** > **次へ**の順に移動します。</span><span class="sxs-lookup"><span data-stu-id="eac89-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="eac89-109">[**起動**] を選択して、PowerShell のトラブルシューティングメニューを開きます。</span><span class="sxs-lookup"><span data-stu-id="eac89-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="eac89-110">**パスワード同期のトラブルシューティング**を選択します。</span><span class="sxs-lookup"><span data-stu-id="eac89-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="eac89-111">通常、特定のユーザーアカウントのパスワードは同期されないことが問題になります。</span><span class="sxs-lookup"><span data-stu-id="eac89-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="eac89-112">**注** 最後に通常にパスワードを同期してから時間が経過している場合は、パスワードを同期できません。</span><span class="sxs-lookup"><span data-stu-id="eac89-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="eac89-113">パスワード同期のトラブルシューティングの詳細については、「[Azure AD Connect 同期によるパスワードハッシュ同期のトラブルシューティング](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="eac89-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>