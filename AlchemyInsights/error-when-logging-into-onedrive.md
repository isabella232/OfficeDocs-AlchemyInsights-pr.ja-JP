---
title: OneDrive の起動時に 0x8004de40 エラーが発生する
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6886"
- "9003837"
ms.openlocfilehash: f689fcf9432e9b356843efe73ed0f79a32735e6f
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 10/30/2020
ms.locfileid: "48823245"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a><span data-ttu-id="62161-102">OneDrive の起動時に 0x8004de40 エラーが発生する</span><span class="sxs-lookup"><span data-stu-id="62161-102">0x8004de40 error when launching OneDrive</span></span>

<span data-ttu-id="62161-103">OneDrive にログインしたときにエラー **0x8004de40** を受け取った場合は、職場または学校のドメインに接続した状態でコンピューターを再起動してください。</span><span class="sxs-lookup"><span data-stu-id="62161-103">If you receive an error **0x8004de40** when  logging into OneDrive, reboot the computer while connected to your work or school domain.</span></span> <span data-ttu-id="62161-104">再起動後にこのエラーが発生した場合は、職場または学校のドメインに接続しているときにこれを試してください。</span><span class="sxs-lookup"><span data-stu-id="62161-104">If you receive this error after rebooting, try this while connected to your work or school domain:</span></span>

1. <span data-ttu-id="62161-105">[スタート] をクリックし、検索ボックスに **cmd** または **コマンド プロンプト** と入力し、コマンド プロンプト アプリを右クリックして、**[管理者として実行する]** を選択します。</span><span class="sxs-lookup"><span data-stu-id="62161-105">Click Start, and type **cmd** or **command prompt**  in the search  box, right-click on the command prompt app, and select  **Run as administrator**.</span></span> <span data-ttu-id="62161-106">管理者のパスワードを要求するダイアログ ボックスが表示された場合はパスワードを入力して [OK] をクリックし、確認を要求するダイアログ ボックスが表示された場合は [**許可**] をクリックします。</span><span class="sxs-lookup"><span data-stu-id="62161-106">If you are prompted for an administrator password or for a confirmation, type the password, or click **Allow**.</span></span>  

2. <span data-ttu-id="62161-107">コマンド プロンプト ウィンドウで、**dsregcmd /leave** と入力し、コマンドが完了するのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="62161-107">In the Command Prompt window, type **dsregcmd /leave**  and wait for the command to complete.</span></span> <span data-ttu-id="62161-108">次に、**dsregcmd /join** と入力し、コマンドが完了するのを待ちます。</span><span class="sxs-lookup"><span data-stu-id="62161-108">Then type **dsregcmd /join** and wait for the command to complete.</span></span>
3. <span data-ttu-id="62161-109">コンピューターを再起動します。</span><span class="sxs-lookup"><span data-stu-id="62161-109">Reboot your computer.</span></span>
