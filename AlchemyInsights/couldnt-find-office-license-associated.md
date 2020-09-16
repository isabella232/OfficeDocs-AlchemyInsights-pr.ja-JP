---
title: Microsoft 365 アプリの「関連する Office ライセンスが見つかりませんでした」メッセージの修正
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
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747700"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="793e6-102">Microsoft 365 アプリの「関連する Office ライセンスが見つかりませんでした」メッセージの修正</span><span class="sxs-lookup"><span data-stu-id="793e6-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="793e6-103">このメッセージが表示された場合は、次を試してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="793e6-104">ファイアウォール、ウイルス対策ソフトウェア、プロキシ設定を確認し、インターネットが Microsoft 365 アプリにアクセスするのをそれらがブロックしていないことを確認します。</span><span class="sxs-lookup"><span data-stu-id="793e6-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="793e6-105">「[Microsoft 365 の URL と IP アドレスの範囲](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="793e6-106">Office ライセンスを削除し、影響を受ける[ユーザーに再割り当て](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)します。</span><span class="sxs-lookup"><span data-stu-id="793e6-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="793e6-107">Office アプリを開き、既存のすべてのユーザー アカウントから[サインアウト](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071)します。</span><span class="sxs-lookup"><span data-stu-id="793e6-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="793e6-108">Windows の設定、[**アカウント**] > [**メールとアカウント**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを削除します。</span><span class="sxs-lookup"><span data-stu-id="793e6-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="793e6-109">Windows の設定、[**アカウント**] > [**職場または学校にアクセスする**] の順に移動し、影響を受けるアカウントを除くすべての職場アカウントを切断します。</span><span class="sxs-lookup"><span data-stu-id="793e6-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="793e6-110">Office のライセンス認証の状態をリセットします。</span><span class="sxs-lookup"><span data-stu-id="793e6-110">Reset the Office activation state.</span></span> <span data-ttu-id="793e6-111">[詳細情報](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="793e6-112">影響を受けるアカウントを使用して[サインイン](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) します。</span><span class="sxs-lookup"><span data-stu-id="793e6-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="793e6-113">その他のトラブルシューティング ソリューションについては、「[Office でのライセンスのない製品エラーとアクティブ化エラー](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)」に関するページを参照してください。</span><span class="sxs-lookup"><span data-stu-id="793e6-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>